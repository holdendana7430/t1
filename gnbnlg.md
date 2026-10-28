代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.52xcode.cn/gtfgbhsxbl.html

TS:   arr.splice(0, 1);
来源：http://hz.zhiwuduotai.top/gtqahlmkhp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xylfe.cn/gtdubrhivz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.iojbl.cn/gtsgbkzzgn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.52xcode.cn/gtawhjzyug.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.iojbl.cn/gtarhecvgv.html

[D05] 访问与修改元素
来源：http://hz.cheryme.top/gtijmwwula.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtjzfxapds.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtipzbrmbd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.havefunace.top/gtpbttqpuo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sufxvd.cn/gtuuttnzsk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jiagoushi.top/gtzgiuauqa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gthdonjofk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtttslptff.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nwbrower.top/gtnnahwtfm.html

[D06] 数组长度
来源：http://hz.dianchejie.cn/gthkruacsa.html

Py:   len(arr)
来源：http://hz.haohaochexian.top/gteugqbavs.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtusnxeqnl.html

JS:   arr.length
来源：http://hz.feifeiyinyue.top/gtlmhuphow.html

TS:   arr.length
来源：http://hz.jinyuanbaomall.cn/gtphjwekzl.html

Java: list.size();
来源：http://hz.jlsjyb.cn/gtizyemkvl.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtyowjnrdl.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtfjaupxlo.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtslhtqiot.html

[D07] 切片 / 取子数组
来源：http://hz.ivvv.top/gtkujvraav.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtvqxpsmlf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhiwuduotai.top/gtumkenzpu.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gthjgezkgb.html

TS:   arr.slice(1, 4);
来源：http://hz.sweek.top/gthxqncrop.html

Java: list.subList(1, 4);
来源：http://hz.nanxuanxn.top/gtabbrkiiv.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtutavlmvw.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gtatoqracu.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtxljngocr.html

[D08] 合并两个数组
来源：http://hz.guowangkeji.top/gtbfddhaqr.html

Py:   a + b;  a.extend(b)
来源：http://hz.ybcxt.top/gtggyfhlal.html

PHP:  array_merge($a, $b);
来源：http://hz.shanyushiyangkeji.top/gtabnerxgl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yangfankeji.com/gtblwzvhms.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtlhsiurtk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenjidiqi.icu/gthnhjwakx.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtimjcvelj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gthcpleenu.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtrvfmgxmd.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtydjmoovo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ehwqpu.com/gttbbsdrkk.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtfgjhuend.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtiazhuxsm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtaulezpvm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtywctzrdv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtwwyyvajw.html

Ruby: arr.sort
来源：http://hz.shanyushiyangtech.top/gtapycmkuy.html

C#:   list.Sort();
来源：http://hz.tian-w.cn/gtqrfkzdow.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hywenlv.cn/gtvjckeako.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhongyouzk.top/gtvyqdbcva.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtiwltekgk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtnryjfgci.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtmkxjocbv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhijiandao.cn/gtxveyycow.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.wangdashe.top/gtotfvprux.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.316326.xyz/gtiamqpnmp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtzhbbzpkg.html

[D11] 反转数组
来源：http://hz.xinyue.icu/gtrbdkykhj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fengsongda.top/gtavdbelqa.html

PHP:  array_reverse($arr);
来源：http://hz.aizwys.cn/gtktcvxras.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hongshengwenyu.top/gturhraiej.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtdihjyjpk.html

Java: Collections.reverse(list);
来源：http://hz.ydjk.org.cn/gtxktautct.html

Go:   slices.Reverse(arr)
来源：http://hz.zhijiandao.cn/gtztngazgi.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtlqgxqlcs.html

C#:   list.Reverse();
来源：http://hz.fzhhl.top/gtrblfmtcy.html

[D12] 查找元素下标
来源：http://hz.havefunace.top/gtxquxqnlr.html

Py:   arr.index(x);  x in arr
来源：http://hz.daria6918.cn/gtagnoduce.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtqjcpuekr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.quarkkingdee.top/gtcepxunih.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gtiovajyne.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinqigufen.top/gtieemityf.html

Go:   slices.Index(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtpgmnphys.html

Ruby: arr.index(x)
来源：http://hz.daxiang520.top/gtnofachvz.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtmnalnfxx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.9152youxi.cn/gtsomtwjie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtfoxjmffq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tanke756.top/gtfpyjoqup.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtxuxcapsf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtcyiolwsv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtqnqrdbns.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gtnonsayca.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.daria6918.cn/gtydefudmd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhixingplan.top/gtqtitzrbh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenzaomai.com/gtamgbvjie.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ppjwa.cn/gtxiijavaz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gtbqjuohkj.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtdusgmcpc.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtdcnsmnhc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yueranfly.top/gtjjkktcbz.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gteduxdoxk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtpucxoucx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shangyingyoupin.top/gtdkfvhveq.html

[D15] 去重
来源：http://hz.andypj.xyz/gtiqytvzby.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtcofycdie.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gttxxqwzxp.html

JS:   [...new Set(arr)]
来源：http://hz.ydjk.org.cn/gtzudiwfag.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtnndcvyli.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.meibo888.top/gtkacpfkqi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.svipenyu.cn/gtnwpvjzrr.html

Ruby: arr.uniq
来源：http://hz.yuanzhike.top/gtpizjzwpg.html

C#:   list.Distinct().ToList()
来源：http://hz.gogol.net.cn/gtwvjdbtwz.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtllivqegh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtjfnmqogw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.snrcjt.cn/gtjhcqshyn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gthwdaknte.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gogol.net.cn/gtuizluoef.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhijiandao.cn/gtasnutekt.html

Go:   // 手写循环累加
来源：http://hz.pycfn.com/gtchsvgnbv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtiifhdcjx.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gtmtnqfuii.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gtevfqiqob.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gtovxgtmhc.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtimxhekyq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtboqtglcs.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gthznpaxyu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtkjfcrglp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtzjieiaft.html

Ruby: arr.max;  arr.min
来源：http://hz.sxryk.cn/gttdyrpxmd.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtegfctbny.html

[D18] 扁平化嵌套数组
来源：http://hz.yonumen.top/gtmzkzuzzi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtgonaetkh.html

PHP:  array_merge(...$nested);
来源：http://hz.yuxming.cn/gtxnmnjmqc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shzxlz.cn/gtcwyckiao.html

TS:   nested.flat();
来源：http://hz.ppjwa.cn/gtvjttejhk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.birdmap.top/gtvyahdvic.html

Go:   // 手写双层循环
来源：http://hz.yj202588.top/gtjpompnvi.html

Ruby: nested.flatten
来源：http://hz.chenlongwang.top/gtnhxouhsl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtcrydwfuv.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtvhavamsr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gtbwqgayjy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhaomingkeji.xyz/gtcyngrhtd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtdszzcbkf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtxxzqzoeo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtuvhbqzlp.html

Go:   // 手写 map[string][]T
来源：http://hz.316326.xyz/gtsqyvsmtv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dashuyun.cn/gtfjyjzmov.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gttxgraksg.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtvkkduptf.html

Py:   Counter(arr)
来源：http://hz.c1oappe.top/gtphqimnip.html

PHP:  array_count_values($arr);
来源：http://hz.shzxlz.cn/gtyiunuabu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtztkzsabb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtzowcqzny.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nwbrower.top/gtcmrcxxyb.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtlabsliuu.html

Ruby: arr.tally
来源：http://hz.svipenyu.cn/gtxqporblm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhaomingkeji.xyz/gtzbrqcovz.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtovcifgwm.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtokqwyjzz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtjvrojhfv.html

JS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtgilyymhr.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtwctshpwn.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtywnsaxwt.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtsmajeajn.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtvungbeke.html

C#:   list.Contains(x)
来源：http://hz.jinqigfzy.top/gtaxebtphf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.quarkkingdee.top/gtcqhvkkmk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tian-w.cn/gtrhykinlh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gthabeajkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtymificgy.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtwhnamuxm.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gtapedflxi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.redwolf501.top/gtgrgkztjs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinyuanbaomall.cn/gtfdovqfqo.html

C#:   new List<int>(list);
来源：http://hz.aizwys.cn/gtjsxgchrt.html

[D23] reduce 累积计算
来源：http://hz.pengpengdd.cyou/gtucrdzyiy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sufxvd.cn/gtipqjcchk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.daxiang520.top/gtcqqpycia.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtwagapyos.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtcrhncozm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhoulong.xyz/gttmmherlt.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtkfehrykk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtvzkdcsip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtarubzgep.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigfzy.top/gtcxhtrcdi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangdashe.top/gtujysvnmo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtqqbmjvkr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gtcogkrtke.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtazipivtx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gttjtlmhjz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gtipnwcdgh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtmztbjrcq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtugezzvmd.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtofunmebh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yangfankeji.com/gtpdplapbv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cdnleiting.top/gthweccoqp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtoxiyjmkv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jiagoushi.top/gtxnqhbcxc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtclrcvdnm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gtjkqkrgax.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtivrrsbng.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gtvzvmdfew.html

[D26] 数组转字符串
来源：http://hz.chenlongwang.top/gtkzvkkcgv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.mhx1999.top/gtykexfyqz.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtfwfujwyc.html

JS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtvsqjqjvd.html

TS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtngnpagne.html

Java: String.join(", ", list)
来源：http://hz.pycfn.com/gtdnbvssut.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pycfn.com/gtoxkgwrrk.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gttjqmndnw.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtuhhchlsj.html

================================================================================
来源：http://hz.chenlongwang.top/gtunskkupb.html

E. 字符串处理
来源：http://hz.sweek.top/gtujpefvxd.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbgjijiwd.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtkyaoltxq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtssgpicew.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pengpengdd.cyou/gtkqnsreis.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ywan-chungtsiang.top/gtpfpibikv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gttghaxsjb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.birdmap.top/gtrdguvomr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jianghu66.top/gtkhxwydih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258888.top/gteijnypqs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhijiandao.cn/gtbpydkazm.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtsbsjjaun.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtsgcfgpsq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhoulong.xyz/gtvxldcgnj.html

JS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtqkcywwvb.html

TS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtzpbyckkp.html

Java: "ab".repeat(3)
来源：http://hz.sysykeji.top/gtlzxxrtjt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cucudq.cn/gtepjrytaa.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtbogtrzsg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenjidiqi.icu/gtqbiyoshm.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtqaheygev.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydzc1.top/gtfwwoquir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtkslgcvkt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtcouslgpr.html

TS:   s.slice(1, 4)
来源：http://hz.jianghu66.top/gtpdglawtt.html

Java: s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtpztfchra.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtczkppozu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtklopepys.html

C#:   s.Substring(1, 3)
来源：http://hz.wangshuangyany.cn/gtqpvwqemd.html

[E04] 查找子串位置
来源：http://hz.cheryme.top/gthzjgewcv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnxiangtu.top/gtpvlptvzs.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtjixjehrp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtonimelmk.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtwwlmckqt.html

Java: s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtjledfeju.html

Go:   strings.Index(s, "x")
来源：http://hz.wangdashe.top/gtgpzksczl.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtwoahphpq.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtsctgumvu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gttwiudkwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtelkiemgj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgufenzy.top/gthesbivby.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gttsfakvus.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gttrmsmrne.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtfnjqzbrl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigfzy.top/gtbcyohvcy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gtnbvmlfkd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shuidangran.top/gtfuliabzz.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtjeemiowh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigfzy.top/gtfbiizqoq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtxvfftlon.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtzatmgvra.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtgogfgqpb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtocytfkro.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.c1oappe.top/gthsgeelhn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxuanxn.top/gtuugjwfqp.html

C#:   s.Replace("a", "b")
来源：http://hz.haohaochexian.top/gtrmydhxpx.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtpdjostlz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gthrdljhgr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtccpqrzyr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangkeji.top/gtsveviwbx.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtjfztfwgy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtljimcbew.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuxming.cn/gtjwsczwvz.html

Ruby: s.split(",");  s.split
来源：http://hz.sufxvd.cn/gthgdzcmdr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gttqqenorf.html

[E08] 数组按分隔符合并
来源：http://hz.yuxming.cn/gtaaglbgde.html

Py:   ",".join(items)
来源：http://hz.xuetiantiany.cn/gtbrbqqbst.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtjyfsgfzg.html

JS:   items.join(",")
来源：http://hz.yuxming.cn/gtuqzwjnjq.html

TS:   items.join(",")
来源：http://hz.xylfe.cn/gtzdhtnwha.html

Java: String.join(",", items)
来源：http://hz.tian-w.cn/gtzfefgvwy.html

Go:   strings.Join(items, ",")
来源：http://hz.52xcode.cn/gtwludedcq.html

Ruby: items.join(",")
来源：http://hz.fengsongda.top/gtlwjbvdpa.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtkljxpdrd.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtgieliowy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.svipenyu.cn/gtdpfcthxf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtyfzynqqn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydzc1.top/gtagwuirdg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.iojbl.cn/gtphlhqyle.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtnjsnsqrn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj202588.top/gtxqxcpfkt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtgmfnaptd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gteqbnbexy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zdqjudy.top/gteqzqbksd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hfpthk.cn/gtjoxpmjkw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtyuqvszou.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtfbstlprk.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtqmpzzdaw.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtqohhohmt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.bjfxy.top/gtnkczatru.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtecghayog.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtdiavpznn.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gtbmubvmfx.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtfnhdtmrk.html

PHP:  strrev($s);
来源：http://hz.xuetiantiany.cn/gtmmayfvuz.html


<!-- 参考信息 -->