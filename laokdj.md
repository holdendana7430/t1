代发 wailian999

Py:   len(arr)
来源：http://hz.xuanzx.com/gtzyrhnpdy.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtnrflurqc.html

JS:   arr.length
来源：http://hz.daxiang520.top/gtjsxtkmqk.html

TS:   arr.length
来源：http://hz.dashuyun.cn/gtfeknibxt.html

Java: list.size();
来源：http://hz.svipenyu.cn/gtfnhulacy.html

Go:   len(arr)
来源：http://hz.c1oappe.top/gtncesjzhc.html

Ruby: arr.length; arr.size
来源：http://hz.dianchejie.cn/gtgqrdluhj.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtcrudxilf.html

[D07] 切片 / 取子数组
来源：http://hz.daria6918.cn/gtyoefxtbz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.fengsongda.top/gtnjmzeyxj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtfjlsxokh.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtjkkveblb.html

TS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtodaodupn.html

Java: list.subList(1, 4);
来源：http://hz.chenzaomai.com/gtgpxpsjwj.html

Go:   arr[1:4]
来源：http://hz.yj20258.top/gtgpmtcusu.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtubpxeqkt.html

C#:   list.GetRange(1, 3);
来源：http://hz.dianchejie.cn/gtjktoqher.html

[D08] 合并两个数组
来源：http://hz.gogol.net.cn/gtfibdgscj.html

Py:   a + b;  a.extend(b)
来源：http://hz.tian-w.cn/gtxtaqhadl.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtqdsczhui.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yueranfly.top/gtyojjhgua.html

TS:   [...a, ...b];
来源：http://hz.yvedp.cn/gtaoueaybo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtvxdbifxo.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gtskoeswif.html

Ruby: a + b;  a.concat(b)
来源：http://hz.mhx1999.top/gtaryguxqy.html

C#:   a.Concat(b).ToList()
来源：http://hz.tianlin.xyz/gtqnzdlmva.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtmoicpops.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gtbfaalnwe.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtlmglkima.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtojkhapih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtmgoaqyhu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.iojbl.cn/gtrddaksvb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtwapaympm.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtasekzmph.html

C#:   list.Sort();
来源：http://hz.guowangkeji.top/gthrahytzm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gthlpcdbdx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gaohongyu789.top/gtlbchoams.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuetiantiany.cn/gtxwsdgvyr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtktamffuv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jyoumei.cn/gtzccoplbz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hfpthk.cn/gtlxgecwdt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtgxegnygq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gtpyqffqmg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtopbujbbd.html

[D11] 反转数组
来源：http://hz.redwolf501.top/gtyxxalkcg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daxiang520.top/gtehmvtume.html

PHP:  array_reverse($arr);
来源：http://hz.0kj1m.cn/gtlxjkovmf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtxnpqdiwz.html

TS:   [...arr].reverse();
来源：http://hz.xuanzx.com/gtaugvplww.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtrisrnnug.html

Go:   slices.Reverse(arr)
来源：http://hz.dashuyun.cn/gtdjrrzgev.html

Ruby: arr.reverse
来源：http://hz.haohaochexian.top/gtlhmcxtai.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtltelmugj.html

[D12] 查找元素下标
来源：http://hz.9152youxi.cn/gthwiiawqz.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gttympnzno.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.9152youxi.cn/gthflnllui.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtorgxkman.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtwiyevhet.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnqzz.top/gtttliliej.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtbadiqjvu.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtzvlknifx.html

C#:   list.IndexOf(x);
来源：http://hz.birdmap.top/gtfqouwxvs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtpfxnyapu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gaohongyu789.top/gtxlzpsrgw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtztpnfbmy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gtltpbbmdu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtgsxdeurv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinyuanbaomall.cn/gttmqjjtgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgufenzy.top/gtimzxsxxd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangkeji.top/gtiqmryytw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtcyrwbcbi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtrdptdgcd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gteegywtjk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gttnimnxzx.html

JS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gttgdfcehw.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtquscrxeg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtrtaufwzs.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtwzakyybi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xingfuxueyuan.xyz/gttsxwmssk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cqqwz.cn/gtmpjthzdq.html

[D15] 去重
来源：http://hz.nanxinkj.top/gtutbaruxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtqdtqoyko.html

PHP:  array_unique($arr);
来源：http://hz.sxryk.cn/gtvkphmjiy.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtcbmlbmpk.html

TS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gturkdqrsa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtinfwmkzs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gtfvrmiwlh.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtplwnsdcr.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtsxcbrabk.html

[D16] 求和与平均值
来源：http://hz.cucudq.cn/gtsxusvaxj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.quarkkingdee.top/gtslmyncco.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258.top/gtzejevxub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtdbizkmxr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangkeji.top/gthynbyihs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangkeji.top/gtvrrikrto.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gtssdpobcv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangdashe.top/gtfthtvgeg.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtlfytjduz.html

[D17] 最大值与最小值
来源：http://hz.hammf.cn/gtabrvemka.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigufen.top/gtfrvogmiy.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtvahruvvp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sufxvd.cn/gtsrceqclc.html

TS:   Math.max(...arr);
来源：http://hz.yueranfly.top/gtpmtjulot.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtjbyejgqc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtgmtsqtxr.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gtpqqvwcrn.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtofrdjwho.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtqvudmmfv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtcfcvctgi.html

PHP:  array_merge(...$nested);
来源：http://hz.smart0.xyz/gtqzupmwec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtmqikqegj.html

TS:   nested.flat();
来源：http://hz.tian-w.cn/gtlqtigjlj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gtyqgtysbi.html

Go:   // 手写双层循环
来源：http://hz.quarkkingdee.top/gtsvliaetz.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtvrjfegxp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ivvv.top/gtmzccvigb.html

[D19] 按字段分组
来源：http://hz.tianlin.xyz/gtdhccsxqe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtngeeclbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtriumxlec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj202588.top/gtjiykjfph.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtxwecrabx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtsvarvkae.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtmrlgilfb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nanxuanxn.top/gtslrjpshb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtlobwzivn.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtrhqsymxl.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtteyktdva.html

PHP:  array_count_values($arr);
来源：http://hz.hywenlv.cn/gtsiibomds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtdlkbxxjz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtkyxbqtdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtxqrxgkia.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtsmwddfyt.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtuueapmdc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtgprukvxv.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtjifqbngs.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtlohsrmnx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenjidiqi.icu/gtqyvgoiem.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtxhyxthth.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtywgwitkt.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gtddlbhnbo.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtahugkxeo.html

Ruby: arr.include?(x)
来源：http://hz.snrcjt.cn/gtevtlzoji.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtibmvmjry.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtlkgaytxw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuetiantiany.cn/gtigzrfvdu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aizwys.cn/gtqadaqsnh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtzbooroml.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtcskjpbxk.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gttmndmcjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtacjsorcw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydzc1.top/gtorlsccwj.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtimnkhxdl.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtcqomjusd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sweek.top/gtfhaaemqb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtofatelrd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtzxaxuqst.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtiizkiazx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtsiwyzvnl.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtrpskevlj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gteojpwsji.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.52xcode.cn/gtcaalhkcl.html

[D24] 字典 / Map 基本操作
来源：http://hz.aibaodan.cn/gtghwlfwso.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtomuosiyd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtdczbvcpy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ivvv.top/gtybmvslhn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gttfpkgbca.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gtcfycoems.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pengpengdd.cyou/gtiyhepfxu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hfpthk.cn/gtexnpukkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gttgczkrkj.html

[D25] Set 集合去重与交并差
来源：http://hz.xinyue.icu/gtyeylnmcn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtjpjpsbpj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shzxlz.cn/gtxrxltkrl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtsmvexjlk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.iojbl.cn/gtehykpojf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ivvv.top/gtoahuvfkr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gtlevlsucu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yuanzhike.top/gttyozfmls.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtyogoccqp.html

[D26] 数组转字符串
来源：http://hz.jlsjyb.cn/gtkopicmwu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtewklohfc.html

PHP:  implode(", ", $arr);
来源：http://hz.yuxming.cn/gtgkwxxqvj.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtrjaziroq.html

TS:   arr.join(", ")
来源：http://hz.316326.xyz/gtljvtgyqh.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtjvzyalmz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.tian-w.cn/gtlwfiljfd.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gteuvdmivo.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtvfgupqgz.html

================================================================================
来源：http://hz.sufxvd.cn/gtpxdwdzls.html

E. 字符串处理
来源：http://hz.nwbrower.top/gtddikfonb.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrkxvkaio.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtylfgnshs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenlongwang.top/gtxmvrvpmd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtoakciuyo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtosuurxwi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtpqkmauuc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtoeletors.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtxypupmil.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gtqwquqxiu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtwiilahwk.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtiwhsmlth.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtzommjuoc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtaeutwzdn.html

JS:   "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtqpfxtoso.html

TS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtqergbwyz.html

Java: "ab".repeat(3)
来源：http://hz.guannengcc.top/gtzjneesor.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtujmzabpl.html

Ruby: "ab" * 3
来源：http://hz.xylfe.cn/gtwkfvcpcl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtdvcahhdp.html

[E03] 截取子串
来源：http://hz.jyoumei.cn/gtzmonglcl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtvgsafdsg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yangfankeji.com/gtsvozmgtd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guannengcc.top/gtddtunwiv.html

TS:   s.slice(1, 4)
来源：http://hz.shangyingyoupin.top/gtkqxyvoih.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtrsftpzrm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xziqi.cn/gthgdpygnw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtjswhjjiv.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gthfshkcui.html

[E04] 查找子串位置
来源：http://hz.yonumen.top/gtbeckkdpa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtvbecywmp.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtoqowhuhs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtjptqsehi.html

TS:   s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtchqtkhld.html

Java: s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtqlkgjuvj.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtgajwrrnq.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gthobevwvw.html

C#:   s.IndexOf("x")
来源：http://hz.dianchejie.cn/gtyixkvkut.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dashuyun.cn/gtajceabvq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yongpay.top/gtsqibvffy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.snrcjt.cn/gtioazbqeu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtvmuofnai.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtkhfsekob.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gtxypzaxzg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.havefunace.top/gtzrgcjaea.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.snrcjt.cn/gtlhiyoudz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daxiang520.top/gtlvzqawro.html

[E06] 替换子串
来源：http://hz.52xcode.cn/gtfvxdnbmx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtntgjzaup.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtzbtpleej.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xziqi.cn/gtvcmynbba.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtsbtygvdd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtwkaotoyd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.0kj1m.cn/gtqynmaacp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtyfmotdlb.html

C#:   s.Replace("a", "b")
来源：http://hz.shanyushiyangtech.top/gtcmseqeek.html

[E07] 按分隔符拆分
来源：http://hz.zhoulong.xyz/gtckokgyip.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cucudq.cn/gtkybpqfse.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yangfankeji.com/gtmxiagsjc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gthnqacxrf.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gtaytrmlet.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhiwuduotai.top/gtwnhjjfyt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhongyouzk.top/gtaucisjck.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtejqfwcke.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jqgufenzy.top/gtgqropoba.html

[E08] 数组按分隔符合并
来源：http://hz.wangshuangyany.cn/gtdbzpaynw.html

Py:   ",".join(items)
来源：http://hz.fzhhl.top/gtdvcbxhxl.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gtypdwvseq.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gtvqrrozfp.html

TS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtydksnutn.html

Java: String.join(",", items)
来源：http://hz.yonumen.top/gtwkshlcdd.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtdmrcfwcz.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gthxdajfqu.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtomgnejji.html

[E09] 去除所有空白字符
来源：http://hz.iojbl.cn/gtyzcaduad.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhaomingkeji.xyz/gtbwlssvcm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sxryk.cn/gtqtjhavpl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtdupynojf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtjgueifpq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinqigfzy.top/gtkqtxyjbf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hysaishi.cn/gtblmdhseo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtvvytdybc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cucudq.cn/gthfkpqcnm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtfvxjlzff.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtakbeozgl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtohcskvum.html

JS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gteljfpppn.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtouxpowei.html

Java: String.format("%03d", 7)
来源：http://hz.hnqzz.top/gtlomvetod.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gttukfgsma.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtmwydkpbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtfsbsfhed.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtjmmjmlyf.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtfttmlnvy.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtlwjkuhqa.html

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtdsnjpdqm.html

TS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtqewdahaz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtmvfgzuqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ivvv.top/gtgomebudm.html

Ruby: s.reverse
来源：http://hz.feifeiyinyue.top/gtseblwlvf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtpiniikjs.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gthkjxlpes.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtcqxlxyjj.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtaidseegq.html

JS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtxijztjka.html

TS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtnktcygpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtxxozhgry.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxuanxn.top/gtydcawddw.html

Ruby: s.count("a")
来源：http://hz.vqdsnc.cn/gtvvpvxzoy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtwebownki.html

[E13] 逐字符遍历
来源：http://hz.chenlongwang.top/gtolvahxlc.html


<!-- 参考信息 -->