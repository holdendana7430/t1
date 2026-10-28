代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ppjwa.cn/gteuwouhiu.html

Ruby: arr.sort
来源：http://hz.xziqi.cn/gtlykqmhab.html

C#:   list.Sort();
来源：http://hz.wangdashe.top/gtothxcood.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigufen.top/gtfzbvtgge.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtbrscpxxl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtzvwnhgml.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtctbreosa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.mhx1999.top/gtoqxwymwh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.svipenyu.cn/gtygcfueev.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtyxxiiryy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinghuilouyu.cn/gtfamjhtai.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtjibfbrsh.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtlmcrufzz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtiillfclu.html

PHP:  array_reverse($arr);
来源：http://hz.ppjwa.cn/gttqqblfdu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sufxvd.cn/gtwdqhusia.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtqutgnukv.html

Java: Collections.reverse(list);
来源：http://hz.c1oappe.top/gtqhhjvcla.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gttzznlugj.html

Ruby: arr.reverse
来源：http://hz.hongshengwenyu.top/gtauilkuia.html

C#:   list.Reverse();
来源：http://hz.nwbrower.top/gtmltrfdnx.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gttfatiztg.html

Py:   arr.index(x);  x in arr
来源：http://hz.cucudq.cn/gtplgpxbqs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gtaieyrylj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.redwolf501.top/gtkldjvceq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtidgzxipr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gtehgwrsfk.html

Go:   slices.Index(arr, x)
来源：http://hz.sxryk.cn/gthgqymwlr.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gtdheldxkr.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtygwbczhl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtfqwrzoai.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guowangkeji.top/gtknvzcygh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtmtteqfyd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtctaowjse.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtbdhedzgd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtudnlmlky.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtrjbeonsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.c1oappe.top/gtzxdquhhp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gthibghely.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinghuilouyu.cn/gtbynybdus.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhixingplan.top/gteteetnfp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtuabohqvl.html

JS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtqeqdgtfk.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtriuybvuq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtnyqrkfxh.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtzkxtjdog.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.0kj1m.cn/gtnytoyjdv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gtanwcxpil.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtvsfxcpif.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtirjsmlru.html

PHP:  array_unique($arr);
来源：http://hz.xinyue.icu/gtsharaywp.html

JS:   [...new Set(arr)]
来源：http://hz.cashguo.top/gtiavtteng.html

TS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtlfbisqkm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxinkj.top/gthtacmwkx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtantgidop.html

Ruby: arr.uniq
来源：http://hz.pengpengdd.cyou/gtwjldherg.html

C#:   list.Distinct().ToList()
来源：http://hz.yanxiufei.cn/gtidacfjhi.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gttpfmvfly.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtlwwscrqq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ehwqpu.com/gtlrppbyhd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtbumbgnit.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jlsjyb.cn/gtvzfqxuns.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tianlin.xyz/gtraxndrqs.html

Go:   // 手写循环累加
来源：http://hz.nanxuanxn.top/gtvvaebels.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hysaishi.cn/gtmkvtcodf.html

C#:   list.Sum();  list.Average()
来源：http://hz.xingfuxueyuan.xyz/gtzggrqtoq.html

[D17] 最大值与最小值
来源：http://hz.zdqjudy.top/gttugvzhao.html

Py:   max(arr);  min(arr)
来源：http://hz.yueranfly.top/gthrbpglfe.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtzpcaurbl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shangyingyoupin.top/gtcrduxflp.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtccfnuttg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtdukcxwgs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtuhzptyok.html

Ruby: arr.max;  arr.min
来源：http://hz.jianghu66.top/gtwwdjvodl.html

C#:   list.Max();  list.Min()
来源：http://hz.cheryme.top/gthmgwnpnu.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtkpdkpnwn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnxiangtu.top/gtiocwnvmq.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtmtmlalmt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gteygwpqwe.html

TS:   nested.flat();
来源：http://hz.xingfuxueyuan.xyz/gtthsbryha.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jyoumei.cn/gthtqgcijn.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gtvseqxfwy.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtomxnmywn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtvyinairg.html

[D19] 按字段分组
来源：http://hz.zhaomingkeji.xyz/gtpgvqcknm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtkrfrmiwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.chenlongwang.top/gtbgajtarq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cashguo.top/gtacjcyfwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtlmraugfw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cdnleiting.top/gtsbgdtbcj.html

Go:   // 手写 map[string][]T
来源：http://hz.xingfuxueyuan.xyz/gtzaxlchta.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtxfbhhhrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtewomidfx.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtsvenqnui.html

Py:   Counter(arr)
来源：http://hz.jlsjyb.cn/gtkuwsyiax.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtjpdjmozh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtfycuxokh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gttfslgzjm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtweqjparj.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gtqofsxpyt.html

Ruby: arr.tally
来源：http://hz.quarkkingdee.top/gteluufeyi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hfpthk.cn/gttimkdqhi.html

[D21] 判断是否包含某元素
来源：http://hz.yueranfly.top/gtzvzewgpo.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtiixckrmg.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnxiangtu.top/gtndzqudkn.html

JS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtqkklgiaz.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtowzslrmw.html

Java: list.contains(x)
来源：http://hz.pengpengdd.cyou/gtkbnhbikc.html

Go:   slices.Contains(arr, x)
来源：http://hz.dianchejie.cn/gtsennqdsz.html

Ruby: arr.include?(x)
来源：http://hz.snrcjt.cn/gtqkhfhhfm.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtvheegpgq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shuidangran.top/gtvddmueaw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtkeldndny.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtjdgzgtln.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtxnkujvxg.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtaagamrxc.html

Java: new ArrayList<>(list);
来源：http://hz.jinghuilouyu.cn/gtbmcdduzw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtqicwzxcc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtpnxouxvx.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtcewkjuji.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtldimugtr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cdnleiting.top/gtoxkthoky.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.redwolf501.top/gtujjzetsz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtbktoooft.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.mhx1999.top/gtbrkcscft.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgufenzy.top/gtkldhcdpn.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtvyeyzlte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtggjzcska.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtxiaecxbe.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtesymmlwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtnyogwvbl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtxzlqljuu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gaohongyu789.top/gtnqjguyui.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtvshabwhy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtkmxhzovx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cqqwz.cn/gtllyrclit.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zdqjudy.top/gtkbmvhhou.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.andypj.xyz/gtzedejrzg.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gtxzdpteut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtqnyymmol.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtdqfkggch.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gthndvctgo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtnlqptfao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtxdtdueje.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yonumen.top/gtjwrvlths.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.quarkkingdee.top/gtaocjpwng.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtxwsmdwbx.html

[D26] 数组转字符串
来源：http://hz.hnxiangtu.top/gtyhvsnacu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gtiooerhmo.html

PHP:  implode(", ", $arr);
来源：http://hz.jianghu66.top/gtxavyhsiu.html

JS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtfqzijvii.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gttosqqkpj.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gtseletwnb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenlongwang.top/gturrrbgfu.html

Ruby: arr.join(", ")
来源：http://hz.jqgufenzy.top/gtipjyswvx.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtfoyjardi.html

================================================================================
来源：http://hz.svipenyu.cn/gtbuylgymk.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gtviwvpeoh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtjvvyhwas.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtgpzsbxqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gttryopkso.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gotoacloud.top/gtdxxkjebj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fzhhl.top/gtjttlbywo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtpznprktp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daxiang520.top/gtflvqsjrr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gtxvoiwrfj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gthdogcyjl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.c1oappe.top/gtfuqmwdud.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gthuzblmep.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtbgzihxcf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pycfn.com/gtyrwteewj.html

JS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gttjfxafwa.html

TS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtegtifsos.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtqmjuxitr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shuidangran.top/gtafkjqids.html

Ruby: "ab" * 3
来源：http://hz.ivvv.top/gtbopxdgxi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuanzx.com/gtzwkasftu.html

[E03] 截取子串
来源：http://hz.cheryme.top/gtjdhqmczq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtqfngdzrb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.kuanghao11.cn/gtmsyvynhp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtcloiwezk.html

TS:   s.slice(1, 4)
来源：http://hz.xinyue.icu/gtxhlgbfcy.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtqaqqprie.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gtuaazxepr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtyjerohkm.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgufenzy.top/gtsdwxylen.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtxwwhecyx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sxryk.cn/gtjzviahjo.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gtxxmfvlgh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cqqwz.cn/gtqytzhogn.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtdwipbpcs.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gtgigrueqk.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtnpnnztfj.html

Ruby: s.index("x")
来源：http://hz.0kj1m.cn/gtngqogcct.html

C#:   s.IndexOf("x")
来源：http://hz.ppjwa.cn/gtegpzrxwz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhoulong.xyz/gtjrzitast.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtcwqhieiz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258888.top/gtwdmluisi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtvmdxnoao.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtbqmoofkr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shuidangran.top/gtwtawokec.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.0kj1m.cn/gtwafygrad.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.birdmap.top/gtdxysbxzj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gtroktgzts.html

[E06] 替换子串
来源：http://hz.xinyue.icu/gtbblgqjpn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yonumen.top/gtaajtjyzz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtaketfchb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtinysvfos.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtrzvindbd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtipgcpwbw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yangfankeji.com/gttbmuatbi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yanxiufei.cn/gtbccrokzl.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtqmasidpl.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gtwnlyojil.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtnivkeyhy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtaskccbtf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daria6918.cn/gtbdsaeucv.html

TS:   s.split(",")
来源：http://hz.yuxming.cn/gtkrxbnsev.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtemmaryoq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangshuangyany.cn/gtibglogvd.html

Ruby: s.split(",");  s.split
来源：http://hz.xuetiantiany.cn/gtlcbwiaht.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gtvexlrxye.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtvlvunicz.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gttyhujhca.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtalmsllwi.html

JS:   items.join(",")
来源：http://hz.zhongyouzk.top/gtbqllrpph.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gtngjnjdtb.html

Java: String.join(",", items)
来源：http://hz.0kj1m.cn/gtbvvxfgyc.html

Go:   strings.Join(items, ",")
来源：http://hz.daria6918.cn/gtqdgmhfkf.html

Ruby: items.join(",")
来源：http://hz.wangdashe.top/gtfjvfzulq.html

C#:   string.Join(",", items)
来源：http://hz.yonumen.top/gtjkmywdlw.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtwblbamvg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jianghu66.top/gtxidvjufx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtfzcjiurv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nwbrower.top/gtmhykrume.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtoqyscfas.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhongyouzk.top/gtwwjbwrqp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hysaishi.cn/gtppwtfcfk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtmkuiyqnn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtzgekarvn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtredkrmod.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hongshengwenyu.top/gtiprlsghd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tian-w.cn/gthqghpajo.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtkaipkbev.html

TS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtggusuifz.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gtgytlxhbo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258.top/gtqytosgoc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.iojbl.cn/gtsldbhlkf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guannengcc.top/gtljoheqci.html

[E11] 反转字符串
来源：http://hz.nanxinkj.top/gtalkbldzb.html

Py:   s[::-1]
来源：http://hz.zhiwuduotai.top/gtugvrnpmy.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtrqbercnd.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtrpeglgtp.html

TS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtbjqpwqsv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.redwolf501.top/gtlhgmobws.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.haohaochexian.top/gtnylolfit.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gtmdjxplhi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sysykeji.top/gtjfzklwgk.html

[E12] 统计某字符出现次数
来源：http://hz.havefunace.top/gtbqdgzidy.html

Py:   s.count("a")
来源：http://hz.tanke756.top/gtangpxbsu.html

PHP:  substr_count($s, "a");
来源：http://hz.chenzaomai.com/gtehkcddet.html

JS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtdvqlujcq.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtkxinxrka.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtorwthgqx.html

Go:   strings.Count(s, "a")
来源：http://hz.tian-w.cn/gtciuomeep.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtzukmupjg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gthoxnsgtu.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangtech.top/gtdysrnkvj.html

Py:   for ch in s: print(ch)
来源：http://hz.ybcxt.top/gthelscxws.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtyyfphdeg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtndakyfzf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtifxljkvn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhengqikj.top/gtwpwfjntw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhongyouzk.top/gtfllolppn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtiiyllxfu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtnwybbqpu.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtnpvtuqrk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtmzkcukjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtafezprad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtofpdysvv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtxwxxfsde.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtqpdejwsx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtraeanjgy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hnxiangtu.top/gtwfuyeekv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtireshbfa.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtxxruouev.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtmrboopyy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydjk.org.cn/gtxzocofro.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinyuanbaomall.cn/gtvxtcqooj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tian-w.cn/gtaqhziirw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shzxlz.cn/gtpofqcuvp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.smart0.xyz/gtjqyhoimx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenjidiqi.icu/gtbasujqpr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xuanzx.com/gtnddxqzbr.html

[E16] 数字千分位
来源：http://hz.shzxlz.cn/gtmfxadyoo.html

Py:   f"{1234567:,}"
来源：http://hz.haohaochexian.top/gtfyvqvaoh.html

PHP:  number_format(1234567);
来源：http://hz.ivvv.top/gtyvzsmcbe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtclwubrzv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtifdipyie.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jiagoushi.top/gtixpkaxhh.html


<!-- 参考信息 -->