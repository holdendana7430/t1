代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangkeji.top/gtkcjayvbn.html

TS:   arr.splice(0, 1);
来源：http://hz.xziqi.cn/gtfbsfkadw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtsycsrkag.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.snrcjt.cn/gthlailmop.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtilsmwuti.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.9152youxi.cn/gthwujgmjj.html

[D05] 访问与修改元素
来源：http://hz.andypj.xyz/gtfkjvaiph.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtwmuleznz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gotoacloud.top/gtweaiistr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.haohaochexian.top/gtizjxunfc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daxiang520.top/gtujpchdpp.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtycqfqwgz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gtospvgpgf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtwxjpprzq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtstyddkoa.html

[D06] 数组长度
来源：http://hz.jianghu66.top/gtfyhcjzhf.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtljxwfits.html

PHP:  count($arr);
来源：http://hz.cashguo.top/gtbrrsifoj.html

JS:   arr.length
来源：http://hz.shanyushiyangkeji.top/gtayxnjsbh.html

TS:   arr.length
来源：http://hz.zhixingplan.top/gtdefbgnvg.html

Java: list.size();
来源：http://hz.daria6918.cn/gtcnmhpdih.html

Go:   len(arr)
来源：http://hz.ivvv.top/gtyolhwhyd.html

Ruby: arr.length; arr.size
来源：http://hz.cucudq.cn/gtkqbllsrk.html

C#:   list.Count;
来源：http://hz.havefunace.top/gtsutosdjl.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gtkeksgpwa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jiagoushi.top/gtfsvgyhsu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtkqitatis.html

JS:   arr.slice(1, 4);
来源：http://hz.ppjwa.cn/gtnytvphrx.html

TS:   arr.slice(1, 4);
来源：http://hz.jyoumei.cn/gtwtykrchn.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtrzlovqci.html

Go:   arr[1:4]
来源：http://hz.cashguo.top/gtquaeogun.html

Ruby: arr[1, 3]
来源：http://hz.jianghu66.top/gtdasntmgt.html

C#:   list.GetRange(1, 3);
来源：http://hz.aizwys.cn/gtmttncdly.html

[D08] 合并两个数组
来源：http://hz.zhiwuduotai.top/gthtknokrx.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gtozveoody.html

PHP:  array_merge($a, $b);
来源：http://hz.yonumen.top/gtfldgphnf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtobvgaugt.html

TS:   [...a, ...b];
来源：http://hz.shangyingyoupin.top/gtkqdfcwzh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hywenlv.cn/gtdtvquocp.html

Go:   append(a, b...)
来源：http://hz.yj20258888.top/gtroepnupa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jlsjyb.cn/gtofgriulz.html

C#:   a.Concat(b).ToList()
来源：http://hz.redwolf501.top/gtbmkycgbj.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gtcjqlvbru.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtzgzrornq.html

PHP:  sort($arr);
来源：http://hz.jiagoushi.top/gtuerhhnho.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.316326.xyz/gtwxxktnju.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtwbzsvumx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.havefunace.top/gtyipvnvcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sxryk.cn/gtbxnpvped.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtlefgbjpt.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtrchwbpgd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinyuanbaomall.cn/gtubcdogkd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtwiwixppm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtwsmjbkaz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtfcdfsdfx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtrtuhqugg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtubeqsnss.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hywenlv.cn/gtvwrjurnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangkeji.top/gtnxielrkf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtrwdbnmfp.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtqyoktolq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtoklxxrmm.html

PHP:  array_reverse($arr);
来源：http://hz.feifeiyinyue.top/gtxsrobzfr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.mhx1999.top/gtjbmzmuck.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtgpecohyz.html

Java: Collections.reverse(list);
来源：http://hz.mhx1999.top/gtkbsheofs.html

Go:   slices.Reverse(arr)
来源：http://hz.svipenyu.cn/gtvbnchqse.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtnbhqhyyg.html

C#:   list.Reverse();
来源：http://hz.hysaishi.cn/gtcvqwloyq.html

[D12] 查找元素下标
来源：http://hz.chenlongwang.top/gtmfjbwfkd.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxuanxn.top/gtbgjdrjjd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.kuanghao11.cn/gtqmmvmzmx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtodrjfnqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtlcodnaqj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtfxrjedkl.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtlflwrcxk.html

Ruby: arr.index(x)
来源：http://hz.guowangkeji.top/gtfdiszeof.html

C#:   list.IndexOf(x);
来源：http://hz.hfpthk.cn/gthenlkfzc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj20258888.top/gtpubxknjb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yvedp.cn/gtgzrbhsyg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtosirppgi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtwcsjzemo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtwmkqagqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhongyouzk.top/gtrvgrxybo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenlongwang.top/gtozniiraq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gtljiktlxl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tianlin.xyz/gttyfybluq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtfzglfnyb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.c1oappe.top/gtnfeertpf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gaohongyu789.top/gtfftkhwwq.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtsicdbqem.html

TS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtlnrrkvln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtvpfgktzm.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtjsxfemcy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.mhx1999.top/gtvsfnrdvx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gtrabdqnbg.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtgbkzgocr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guowangkeji.top/gtfptntyqo.html

PHP:  array_unique($arr);
来源：http://hz.cucudq.cn/gtipvhondu.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtllhcviei.html

TS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtfsayqjlc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhixingplan.top/gthewqyfhz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtghpkjqjc.html

Ruby: arr.uniq
来源：http://hz.cheryme.top/gtotqyucyr.html

C#:   list.Distinct().ToList()
来源：http://hz.ywan-chungtsiang.top/gtinrfwzsv.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gteywmojnb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtqpwjdmrm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.aibaodan.cn/gtbtytmzoc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtkafejrcd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtmtpjsbyz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gtjspqeusk.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtgqxeecsx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gzhubu.top/gtbwpgcpas.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtmqvsxoef.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtkwbwnyib.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigufen.top/gtbdondryw.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtbwkpsvlv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gtcqwjqwsp.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gtyxyvwdnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hfpthk.cn/gtwqkawddu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.feifeiyinyue.top/gthtwpgkzc.html

Ruby: arr.max;  arr.min
来源：http://hz.jinyuanbaomall.cn/gtvmfcqvle.html

C#:   list.Max();  list.Min()
来源：http://hz.yvedp.cn/gtemkaxdhp.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtgwjvlzfe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jinghuilouyu.cn/gtfvbmroih.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtsjzhgabi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtzaljrzga.html

TS:   nested.flat();
来源：http://hz.shanyushiyangkeji.top/gtzrkttgwr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangtech.top/gtltjkrllh.html

Go:   // 手写双层循环
来源：http://hz.316326.xyz/gtvyfwrsto.html

Ruby: nested.flatten
来源：http://hz.shangyingyoupin.top/gttttjdmli.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aibaodan.cn/gtfzrbzxcb.html

[D19] 按字段分组
来源：http://hz.0kj1m.cn/gtyfsodmyn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtccmikpjt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhengqikj.top/gtcpbemvyu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtdcqajwwt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gttqzbfuxy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yongpay.top/gtomteooeg.html

Go:   // 手写 map[string][]T
来源：http://hz.wangdashe.top/gtlsaonvzh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtvwhspvun.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtrbmtrxmk.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtahhejihc.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gtgnlhmolh.html

PHP:  array_count_values($arr);
来源：http://hz.yongpay.top/gtooxqihcm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtnkugtdkb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtzmtrroxk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtxwmmlcko.html

Go:   // 手写 map[T]int
来源：http://hz.jianghu66.top/gtdcnmthvh.html

Ruby: arr.tally
来源：http://hz.jqgufenzy.top/gtxmxlkvlv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtqboktdtm.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigfzy.top/gttutyhzhd.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtsusiouoy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jianghu66.top/gtadeckitw.html

JS:   arr.includes(x)
来源：http://hz.nanxuanxn.top/gtgyupizcx.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gtafhwmefa.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtpdbuhamk.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtvdbgdinu.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtbrpnqrua.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtazqmitjm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guannengcc.top/gtxpmgztjd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.316326.xyz/gthfxbkias.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tian-w.cn/gtvtgofnmv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtmcqsoviq.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtnfhkhgnh.html

Java: new ArrayList<>(list);
来源：http://hz.jinghuilouyu.cn/gtnrdmapky.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtngevskad.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnxiangtu.top/gtrtppmfxw.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtvoytlgyb.html

[D23] reduce 累积计算
来源：http://hz.tanke756.top/gtrhnshjby.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtucdqhhgm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jlsjyb.cn/gtuqrpmyqe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtmporihwd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtkmkgvbjk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gthnhivqkn.html

Go:   // 手写循环
来源：http://hz.smart0.xyz/gtxscmxhfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtsepnzxva.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.9152youxi.cn/gtigahnixi.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gtniurcobi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtkvpzmfkh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ivvv.top/gtuuaqdchv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtlnjacwis.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtohodlyia.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jianghu66.top/gtyehiiyje.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ydzc1.top/gtbijofkvp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jianghu66.top/gtbjrlqhjx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtpfxxpcsi.html

[D25] Set 集合去重与交并差
来源：http://hz.shangyingyoupin.top/gtvrjjqvjo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgufenzy.top/gtjqibkmfg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtmenfxjvj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gttgnabrqw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenlongwang.top/gthvmrixll.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jiagoushi.top/gtgrgjycmt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtrwohmlfm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtcurlpphh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtlhorhdly.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtvymlwjhk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtdazwodax.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtjiejqrjs.html

JS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtilqrocbh.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtiqjcfbqn.html

Java: String.join(", ", list)
来源：http://hz.bjfxy.top/gtryyjayqx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhijiandao.cn/gtfzezqmta.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtervardtv.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtxmjuzrrz.html

================================================================================
来源：http://hz.xuanzx.com/gtkmkkldxv.html

E. 字符串处理
来源：http://hz.gaohongyu789.top/gtyrcffgym.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjwqqsemg.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtejlndtwi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ppjwa.cn/gtuzyowxhz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hywenlv.cn/gtcniyauif.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtozmfhkic.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtcvrjzzhi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtdiazeaxl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shuidangran.top/gttapliebv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gtidqruwrf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.quarkkingdee.top/gteqkadrrf.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gtmlymjfzj.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gtvzfgzeib.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtxlkstcjn.html

JS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtpyxrngns.html

TS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gttypwlzgo.html

Java: "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtihzfqaig.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtsnizooji.html

Ruby: "ab" * 3
来源：http://hz.yangfankeji.com/gtrfsclkko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shangyingyoupin.top/gtrauhflgw.html

[E03] 截取子串
来源：http://hz.yj20258888.top/gtjplnacwq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.chenjidiqi.icu/gtmhuopiwy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gtjsoulvam.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yonumen.top/gtdlzaootv.html

TS:   s.slice(1, 4)
来源：http://hz.hongshengwenyu.top/gtokclmfrh.html

Java: s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtvwpipnwu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.52xcode.cn/gtnoqfglqj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtffdlnipp.html

C#:   s.Substring(1, 3)
来源：http://hz.hfpthk.cn/gtgerzbsrj.html

[E04] 查找子串位置
来源：http://hz.aizwys.cn/gtepgqemfg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj202588.top/gtmzqndvvj.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigufen.top/gtfkpcyxyy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gotoacloud.top/gtqhcbvzhd.html

TS:   s.indexOf("x")
来源：http://hz.nwbrower.top/gtrhyieoog.html

Java: s.indexOf("x")
来源：http://hz.guannengcc.top/gtlmhuyney.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtfgmbtvin.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtxswhcrch.html

C#:   s.IndexOf("x")
来源：http://hz.ehwqpu.com/gtvieipyvf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258.top/gtbdtsbyax.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yonumen.top/gtrspkovwx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yanxiufei.cn/gtnlnixtcl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtzqzhtjdh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.redwolf501.top/gtjnmjxvmr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtfiecttvv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhaomingkeji.xyz/gtolvqqrla.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinghuilouyu.cn/gtuwljjuzm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhengqikj.top/gtktqvajbv.html

[E06] 替换子串
来源：http://hz.vqdsnc.cn/gtedneqbps.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtppsadrfc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhoulong.xyz/gttnsnbwmn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtautfemap.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gthcqmwkws.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtfepvzpmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gtebiooxhv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fengsongda.top/gtxcbrkbqa.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtwucagdqd.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtercjxayg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sufxvd.cn/gtkpvpcypm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhiwuduotai.top/gttgiqwala.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtkwkctpcp.html

TS:   s.split(",")
来源：http://hz.hywenlv.cn/gtzjyoipah.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.52xcode.cn/gtnicyurmt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenlongwang.top/gtsdsbzgvt.html

Ruby: s.split(",");  s.split
来源：http://hz.hywenlv.cn/gthdhtfnal.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258888.top/gtkhxqruih.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtneyrwbvr.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gttidtsmld.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtvogthjiy.html

JS:   items.join(",")
来源：http://hz.mhx1999.top/gtbrmwoqes.html

TS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtoqmzcvcn.html

Java: String.join(",", items)
来源：http://hz.zhaomingkeji.xyz/gttytwcjdy.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtwrwjcdru.html

Ruby: items.join(",")
来源：http://hz.haohaochexian.top/gtjnibiofx.html

C#:   string.Join(",", items)
来源：http://hz.sysykeji.top/gtbtmqbuou.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtcwwxstky.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtkrembvqx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtrwzxwgtg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gteswxlkqu.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtnqnyhuwt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtbnejlhie.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shangyingyoupin.top/gtidszwbnr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenjidiqi.icu/gtpdgbxixx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtezpyjhmz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nwbrower.top/gtjjnieasx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtyztcpppp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hammf.cn/gtnpvybmam.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtcxpcmbeh.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtyppwrovx.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gturzrqidp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtausvclrj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtdrkjdjkx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fzhhl.top/gtmkcbtgbl.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtwhrqhssk.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtqyrsalyr.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gtchrgcpzj.html


<!-- 参考信息 -->