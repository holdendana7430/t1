代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangdashe.top/gtumdrcxem.html

Ruby: arr.sort
来源：http://hz.xylfe.cn/gtcbivbjgc.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gtqtcggazk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hnxiangtu.top/gtpupvoick.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ywan-chungtsiang.top/gthrnayuqt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtopecprnp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.birdmap.top/gtfybgrtnv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtbecctgoe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtzkhhmuuq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtcftkvxao.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuxming.cn/gtojfswrpv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtvuiozmdl.html

[D11] 反转数组
来源：http://hz.zdqjudy.top/gtcyygkxyl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhiwuduotai.top/gtkwljrgwh.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtoykxzbeq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangtech.top/gtwugiflso.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtwjzshbru.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtevyymjfj.html

Go:   slices.Reverse(arr)
来源：http://hz.hfpthk.cn/gtielunyfa.html

Ruby: arr.reverse
来源：http://hz.redwolf501.top/gtfexogzsj.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtpoorjxdl.html

[D12] 查找元素下标
来源：http://hz.daxiang520.top/gtpzdkmwxm.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenjidiqi.icu/gthowgwyqh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhongyouzk.top/gtsmeopjgm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtrqusvtfa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtdjuuuixg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jianghu66.top/gtwnftjwox.html

Go:   slices.Index(arr, x)
来源：http://hz.yuxming.cn/gtcjojehoq.html

Ruby: arr.index(x)
来源：http://hz.nanxuanxn.top/gtkcqcjpeq.html

C#:   list.IndexOf(x);
来源：http://hz.bjfxy.top/gtqxholqat.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtzgvbcehm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cdnleiting.top/gtemxomskv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.quarkkingdee.top/gtmqnwxjhy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtjtprzpus.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fengsongda.top/gttwcedvcy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gtdizxbdpa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtxdurempo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yangfankeji.com/gtxsxrjigo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gtdluqkbxg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtjyktmzwe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhiwuduotai.top/gtsyvsibid.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtemodhgmx.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtnxmzipwa.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhengqikj.top/gtneppzsot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sweek.top/gthpluajto.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtyzwtncvo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtkerpeejt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtsivbfmft.html

[D15] 去重
来源：http://hz.yvedp.cn/gtttqqtesr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtozavpjny.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtsnkcbfvk.html

JS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gtjjctbhuv.html

TS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtzgpirpyu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtgikltmqc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtqjamorqt.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtjvqfhyli.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtotiwqdug.html

[D16] 求和与平均值
来源：http://hz.kuanghao11.cn/gtxyddehoc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.daxiang520.top/gtariryclw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtkkixgcyz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtnpuqkiyc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtsfaqatns.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jiagoushi.top/gtciefrmad.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtdgsvjvnx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtannjmtkp.html

C#:   list.Sum();  list.Average()
来源：http://hz.cheryme.top/gtplrglsoo.html

[D17] 最大值与最小值
来源：http://hz.yj20258888.top/gtpuromfor.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtttfsrfwa.html

PHP:  max($arr);  min($arr);
来源：http://hz.fzhhl.top/gtnjdbzgoc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sxryk.cn/gtikftylun.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtwaiaowsf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtseosthlj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cqqwz.cn/gtbyqwacev.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtjxtfxlli.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtbbiyjejj.html

[D18] 扁平化嵌套数组
来源：http://hz.pengpengdd.cyou/gtdozbymho.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.kuanghao11.cn/gtxgsefdwg.html

PHP:  array_merge(...$nested);
来源：http://hz.wangdashe.top/gtvkptkvnn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtnqdcquxc.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtlmmzzrve.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtbodokqta.html

Go:   // 手写双层循环
来源：http://hz.yuanzhike.top/gtlajhyvfd.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtglkhsqqu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtkrduowdt.html

[D19] 按字段分组
来源：http://hz.snrcjt.cn/gtsrguvwff.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhoulong.xyz/gtygzhmjdw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.daxiang520.top/gtcjgxbupg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gtptsbmljx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtxzmvowkk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangkeji.top/gtpqmonqhe.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtaxbkskwj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtzajbxuoo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258888.top/gtewvkctwc.html

[D20] 统计每个元素出现次数
来源：http://hz.fengsongda.top/gtjsxadckf.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtbmbspftz.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtwdmtolkd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtnkwvhyjf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtmntbwjrm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtzmzvkqad.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gtzpojacye.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gtssiilcrd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtjsnleacc.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtqgrbsgbf.html

Py:   x in arr
来源：http://hz.sweek.top/gtrafldqex.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gthmvujgdh.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtviblnnfz.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtudxlsnpv.html

Java: list.contains(x)
来源：http://hz.shangyingyoupin.top/gtfdorjlev.html

Go:   slices.Contains(arr, x)
来源：http://hz.zycfv.cn/gtvhclknbw.html

Ruby: arr.include?(x)
来源：http://hz.feifeiyinyue.top/gtiohwzzzs.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gteaybrgba.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258888.top/gtkinguaxo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ybcxt.top/gtomzmdubv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.havefunace.top/gtukxkgpfp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yonumen.top/gtzfjfltlv.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtjenmobpq.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gteoltvnge.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtvljwqojp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ehwqpu.com/gtyqxlzchd.html

C#:   new List<int>(list);
来源：http://hz.zhengqikj.top/gtoozdveqq.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gtybhovzek.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dianchejie.cn/gtvdiwcmol.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.9152youxi.cn/gtllctswql.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtykrtbnqj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtjrszzbkq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shuidangran.top/gtirycusxo.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtavcgaqvw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtbsoalbur.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtncfxezxy.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtvnwxbciw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtemwbymox.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gtbakuilpj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtzxeghgdw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtqmltuyfr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gtyhyvmrrl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtxuhscxyy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtfqocyksp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtvxiumjov.html

[D25] Set 集合去重与交并差
来源：http://hz.shuidangran.top/gtrrcterdz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtvsbnhize.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gthqxzjdgl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenjidiqi.icu/gtiarupmgd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtrqrjbyuf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtsmatlyit.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenjidiqi.icu/gthkbshfkj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gtytcjolvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.kuanghao11.cn/gtgdhrnptz.html

[D26] 数组转字符串
来源：http://hz.nanxuanxn.top/gtombmyrud.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtfhtlgryj.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangtech.top/gtwvrplkwt.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtrmlbuyzn.html

TS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtnvgrwraw.html

Java: String.join(", ", list)
来源：http://hz.guowangkeji.top/gtpuqcqsin.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shzxlz.cn/gtkvqdfrsa.html

Ruby: arr.join(", ")
来源：http://hz.yongpay.top/gtmadhgnsx.html

C#:   string.Join(", ", list)
来源：http://hz.yongpay.top/gtmmdjgkee.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzisjfyfi.html

E. 字符串处理
来源：http://hz.zycfv.cn/gthiaovlee.html

================================================================================
来源：http://hz.yj20258888.top/gtzukxyxrw.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtbsrcjulv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gtrjfqbtim.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gtnwppnaju.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtvymdcdlg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gterdbhuek.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgfzy.top/gtbawzbqkw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tanke756.top/gtkldysjqf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtkcwfjhtj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ehwqpu.com/gtwcckubty.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtlvkpoefd.html

Py:   "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtdeibkwdq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtmtkhktuq.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtritgsbak.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtihkbkyyb.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gtgjbkyopk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ehwqpu.com/gtkzavliie.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtmcyrodfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gtizxaweky.html

[E03] 截取子串
来源：http://hz.hywenlv.cn/gtakkuijjm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenlongwang.top/gtvrqaqlrg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gttlnudcby.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtkbaiwijx.html

TS:   s.slice(1, 4)
来源：http://hz.gzhubu.top/gtwtbwzmfd.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtwekkeirb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jianghu66.top/gtfenfrowa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hongshengwenyu.top/gtyotgrmau.html

C#:   s.Substring(1, 3)
来源：http://hz.mhx1999.top/gtatvrjksy.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gtunzbcdhc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtcuwvzqiq.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtayhwnsjo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.bjfxy.top/gtvqhjhnjt.html

TS:   s.indexOf("x")
来源：http://hz.jyoumei.cn/gtuamzlrhf.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtczbaikka.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtwwpmxxui.html

Ruby: s.index("x")
来源：http://hz.pengpengdd.cyou/gtkylxxqqd.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtdvujcsmj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtzytlhhff.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ehwqpu.com/gtfnkoncab.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangkeji.top/gtrvxykglf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtnyknqerx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtzrxdgduz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.havefunace.top/gtvjrdbrdv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhoulong.xyz/gtemidnrfg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtbjffewoi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gtxclcgnth.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtdmfzfdmm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.52xcode.cn/gtnkibpzbi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ivvv.top/gtigxvmzhj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtvqdxalpa.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtowredmmn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtehfgzgjl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtfhqlibgr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtndssozzu.html

C#:   s.Replace("a", "b")
来源：http://hz.jlsjyb.cn/gtrlmwygzv.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gtmytxpbqy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtxosgbhbv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gtzwqsydtm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jlsjyb.cn/gtjyhrsuhp.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gthqwabqrz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gotoacloud.top/gtloswnlaq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.dianchejie.cn/gtfzkadiqi.html

Ruby: s.split(",");  s.split
来源：http://hz.yuanzhike.top/gtndqxuebq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtxbdqkidx.html

[E08] 数组按分隔符合并
来源：http://hz.feifeiyinyue.top/gttlpxqsbo.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtutymmplr.html

PHP:  implode(",", $items);
来源：http://hz.hysaishi.cn/gtzakhccfv.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtfmxstnvh.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtbogpeyea.html

Java: String.join(",", items)
来源：http://hz.bjfxy.top/gtqbtkiupw.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtejkleifl.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtkdanumyn.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtcgtoeaeu.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtntxckliz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yongpay.top/gtkjpvrvat.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtbhpdswml.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtmzdeuykk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtdgzhrwjj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.snrcjt.cn/gtxzweujzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.316326.xyz/gtpgzvkzyc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhengqikj.top/gtguxesltv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtdqootpks.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hywenlv.cn/gtjmezfdcj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtjqepwebp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtwszyizzi.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtlsnttoof.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtawvtwqqn.html

Java: String.format("%03d", 7)
来源：http://hz.guowangkeji.top/gtjqdncgps.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shuidangran.top/gtvrhrskjo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zdqjudy.top/gtfbdebhlr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nwbrower.top/gtuveleqyq.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gteqplvkcu.html

Py:   s[::-1]
来源：http://hz.daxiang520.top/gtseiaqvej.html

PHP:  strrev($s);
来源：http://hz.sysykeji.top/gteihxrwpd.html

JS:   [...s].reverse().join("")
来源：http://hz.mhx1999.top/gtyyvnkrpm.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtamqtthul.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtyttpsfle.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aizwys.cn/gtsbwnoueh.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtxtdlmzgz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtnjqhtkrv.html

[E12] 统计某字符出现次数
来源：http://hz.nanxinkj.top/gttqzzesmr.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtrrijsfrz.html

PHP:  substr_count($s, "a");
来源：http://hz.quarkkingdee.top/gtsubptkin.html

JS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtlhqmqacq.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtovwysonc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtgcrsutlh.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gttwekmhoc.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtpyhhmoit.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtbmglprxx.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtqhbmtrua.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtibrozsfn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.snrcjt.cn/gtowykvnzl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtzncpdyen.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtmnhckwtk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.9152youxi.cn/gtprxkiorv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtljnycrlc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtrsxhvsoe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtlfwjzuqr.html

[E14] URL 编码与 Base64
来源：http://hz.xziqi.cn/gtbvknfdbp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtbpknplnf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinghuilouyu.cn/gtdujmfuep.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hongshengwenyu.top/gtqmbpnlks.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtyhqrognq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtdnjwvmug.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtqxglnvce.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtjmfrknos.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xylfe.cn/gtidgzolrz.html

[E15] HTML 转义 / 反转义
来源：http://hz.cucudq.cn/gtubwcgypq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hongshengwenyu.top/gtsghhnagj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gthgailxsd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhengqikj.top/gtnocueuwb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cashguo.top/gtcrxlzfkh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.birdmap.top/gtrufcxpwn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtwgwfyjso.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtnkmvhyht.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhongyouzk.top/gtlrujkzab.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtdtrzpjpw.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangkeji.top/gtltozyryt.html

PHP:  number_format(1234567);
来源：http://hz.aibaodan.cn/gtotdukkaw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtuvbjjqyp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gttptjihfd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aibaodan.cn/gtjfrcakcu.html


<!-- 参考信息 -->