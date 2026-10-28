代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.wangdashe.top/gtdigglkqi.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtxgliuayt.html

C#:   list.Sort();
来源：http://hz.yvedp.cn/gtxuyiquia.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtvragrjwt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.birdmap.top/gtjqcuihnb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pengpengdd.cyou/gtisptljzr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gthfgchwht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtwxwcdkqf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gthtvdrpnc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gthfemtvpj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gaohongyu789.top/gtxhuydlqe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.pycfn.com/gtdukmqjwx.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gttnpxbjnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtodgfdiaq.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtoqjasdcb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gttzcxomho.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtyachmbbv.html

Java: Collections.reverse(list);
来源：http://hz.tianlin.xyz/gthwejnvuj.html

Go:   slices.Reverse(arr)
来源：http://hz.gotoacloud.top/gtnkyywxzj.html

Ruby: arr.reverse
来源：http://hz.sysykeji.top/gtwffbaqtl.html

C#:   list.Reverse();
来源：http://hz.pengpengdd.cyou/gtuzhapuzd.html

[D12] 查找元素下标
来源：http://hz.xziqi.cn/gtczhlcsmq.html

Py:   arr.index(x);  x in arr
来源：http://hz.yuanzhike.top/gtvxwzkhcq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xinyue.icu/gtvamjepuf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtovnrvufu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtugfyorvd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtuxvcvgcy.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtobzuavca.html

Ruby: arr.index(x)
来源：http://hz.jlsjyb.cn/gtwcejqxgm.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtfpkvuuhs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yangfankeji.com/gtbjwdknaf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hywenlv.cn/gtwjhfhdbb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gthbcfbqje.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gtybamdjml.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtswwyitbk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigufen.top/gtlsnqrfjf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhijiandao.cn/gtwbfjyqsn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuxming.cn/gtczrmwztf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.meibo888.top/gtwdtoakje.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fzhhl.top/gthtiqicga.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtyffvgaeu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gttzhbxzij.html

JS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtmsmarkis.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtvshfypci.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtmunqgcrd.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gthkrhtuvi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtrcmjnmxo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.316326.xyz/gtbvnqiwce.html

[D15] 去重
来源：http://hz.jinghuilouyu.cn/gtgbpczqlj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangtech.top/gttjumgmwl.html

PHP:  array_unique($arr);
来源：http://hz.feifeiyinyue.top/gtoxtdamtb.html

JS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtlwztlhbe.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtfspqxfno.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtrwmbpwru.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gtpatsvazg.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtpnjdjyuh.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtgizfddyu.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtqzqjsckf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gtbbqrjhkl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtfxsurzqf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtpjmuylfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gttfxgipsr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhaomingkeji.xyz/gtyuvwxzap.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtsneoxyuh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtwlitkniq.html

C#:   list.Sum();  list.Average()
来源：http://hz.yvedp.cn/gtsluyntsf.html

[D17] 最大值与最小值
来源：http://hz.birdmap.top/gtuyyizvqp.html

Py:   max(arr);  min(arr)
来源：http://hz.yongpay.top/gtbyvwcyjw.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtsjjjmjfk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.fengsongda.top/gtmecgfmvy.html

TS:   Math.max(...arr);
来源：http://hz.jinghuilouyu.cn/gtasklpmhf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtwveewefm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtyjzrfjym.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gterdgsgiu.html

C#:   list.Max();  list.Min()
来源：http://hz.cheryme.top/gtrfivwrcf.html

[D18] 扁平化嵌套数组
来源：http://hz.hywenlv.cn/gtehqimorz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gtirwoeucy.html

PHP:  array_merge(...$nested);
来源：http://hz.xuanzx.com/gtjxrtwkxf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.bjfxy.top/gtrhkgdqec.html

TS:   nested.flat();
来源：http://hz.9152youxi.cn/gtcvciuwfs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aibaodan.cn/gtawehldkz.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gttcuclrrc.html

Ruby: nested.flatten
来源：http://hz.snrcjt.cn/gtjkxxclwe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtimkowwtw.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtzebwkwnw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtqmnctkgz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtdwjlmffi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtaxvbneqr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangkeji.top/gtlwagypwy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenzaomai.com/gtrxwakvfx.html

Go:   // 手写 map[string][]T
来源：http://hz.vqdsnc.cn/gtkabbksls.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtkuhytwcj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigfzy.top/gtoltexarl.html

[D20] 统计每个元素出现次数
来源：http://hz.cashguo.top/gtadmjnwax.html

Py:   Counter(arr)
来源：http://hz.nanxinkj.top/gtjhcalueu.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtrasqvtos.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gthtkeakkx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtdaduakdd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gtowvanqiv.html

Go:   // 手写 map[T]int
来源：http://hz.52xcode.cn/gtnluorldt.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtocgdbefz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtlfgrckgb.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtvsixezhw.html

Py:   x in arr
来源：http://hz.zhijiandao.cn/gtcabormoc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tanke756.top/gtcprcatfd.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtjzqpaarr.html

TS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtzytmdlzl.html

Java: list.contains(x)
来源：http://hz.jinqigufen.top/gtrdgyctgo.html

Go:   slices.Contains(arr, x)
来源：http://hz.yonumen.top/gtsfiojprf.html

Ruby: arr.include?(x)
来源：http://hz.ivvv.top/gtesyosftj.html

C#:   list.Contains(x)
来源：http://hz.cashguo.top/gtoaualuoh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtvxbtdofp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtuexzsodx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtqcnwzcig.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nanxinkj.top/gtjncmmxey.html

TS:   [...arr];
来源：http://hz.jqgufenzy.top/gtegxhfggu.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gtlnvmndoe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gtsxtfzdij.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtnasngnnw.html

C#:   new List<int>(list);
来源：http://hz.jiagoushi.top/gtkpnajrxz.html

[D23] reduce 累积计算
来源：http://hz.ppjwa.cn/gtkoraxzot.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtbrhezeha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gtctixflkb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtvbxveror.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtxhhkjmsc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jianghu66.top/gtxlgxrguz.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtzatlmxqm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gtuusrbpby.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtjucsorok.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtpocyibll.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.daria6918.cn/gtqtnutzax.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daria6918.cn/gtmtaduwgu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dashuyun.cn/gtnabjojdn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.bjfxy.top/gtawsnskaf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtzlkfyrcz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gtiqzgtajl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gtwjvegbge.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nanxuanxn.top/gtepofosab.html

[D25] Set 集合去重与交并差
来源：http://hz.c1oappe.top/gtgnhmkzly.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtktagwpvd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hongshengwenyu.top/gtleksjvth.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.0kj1m.cn/gtbixeofwl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtwdfkkglu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shuidangran.top/gtuekbkjsn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gtemmqdajn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtitlmdqrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.0kj1m.cn/gtfvmkhqmu.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtunduroya.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtrdmhmzrs.html

PHP:  implode(", ", $arr);
来源：http://hz.ehwqpu.com/gtykmpcejh.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtpkzolnuv.html

TS:   arr.join(", ")
来源：http://hz.cucudq.cn/gttzsadugb.html

Java: String.join(", ", list)
来源：http://hz.gogol.net.cn/gtlwukekfd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtupfwobco.html

Ruby: arr.join(", ")
来源：http://hz.sweek.top/gtcxynwbud.html

C#:   string.Join(", ", list)
来源：http://hz.hammf.cn/gtpctifkdg.html

================================================================================
来源：http://hz.jiagoushi.top/gtqnxbejqs.html

E. 字符串处理
来源：http://hz.chenzaomai.com/gtgrjogtuv.html

================================================================================
来源：http://hz.ybcxt.top/gtyhundicd.html

[E01] 拼接字符串
来源：http://hz.fzhhl.top/gtwdadfkqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtiiylssrj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtsoarvgwh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtujahciph.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtdfxrcknr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtbibchows.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtqmijijnq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gttaansqpp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.haohaochexian.top/gtsngdtmae.html

[E02] 重复字符串
来源：http://hz.ehwqpu.com/gtrlefljjn.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtjggvlsvt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.0kj1m.cn/gtrnzgdmpt.html

JS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtnbqugcvr.html

TS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtvdmflqwl.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gtqzdhglte.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.meibo888.top/gtxqfxoozh.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtuloygnux.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gtinlglfha.html

[E03] 截取子串
来源：http://hz.jiagoushi.top/gtqelpxoxy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gtwkyoknjh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shzxlz.cn/gtzwcrkegp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gtxrkuqbge.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtdtsqvqbs.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gtytertznc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtbtdjoedi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.pycfn.com/gtvhfnwzzj.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangkeji.top/gtdisrzijg.html

[E04] 查找子串位置
来源：http://hz.nanxinkj.top/gtbdlrnszd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.iojbl.cn/gtvuljbemc.html

PHP:  strpos($s, "x");
来源：http://hz.zhoulong.xyz/gtydvmoyrl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangkeji.top/gtizdlkdah.html

TS:   s.indexOf("x")
来源：http://hz.havefunace.top/gtmniewqxh.html

Java: s.indexOf("x")
来源：http://hz.quarkkingdee.top/gtladydjwq.html

Go:   strings.Index(s, "x")
来源：http://hz.meibo888.top/gtldmedadx.html

Ruby: s.index("x")
来源：http://hz.guowangkeji.top/gtmaqmbjod.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtqbxmzqkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xinyue.icu/gtnaumluib.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yvedp.cn/gtnjbbwakl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtsqhdzcxh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtxsdoaylf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtwkwoqmjb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtwkvsjdst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinyuanbaomall.cn/gtycxupxie.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.c1oappe.top/gtuinlyqoy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtyhzcjuzq.html

[E06] 替换子串
来源：http://hz.jinghuilouyu.cn/gtqacfrzji.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtvbbkzwyi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tian-w.cn/gtkzghvcmf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtadlsinmr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtfholydfq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtpqcmrezl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtisrzeuha.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yongpay.top/gtiakdzrvo.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtzqakhgfi.html

[E07] 按分隔符拆分
来源：http://hz.pengpengdd.cyou/gtqfybgecl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.tianlin.xyz/gtivszcsdx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tian-w.cn/gtgnrodipf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtdvgfssfo.html

TS:   s.split(",")
来源：http://hz.c1oappe.top/gthrqppswa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtnmjhkqos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gttochuljq.html

Ruby: s.split(",");  s.split
来源：http://hz.guowangkeji.top/gtkogatrno.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ivvv.top/gtgoyhzpvb.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtwblllwcm.html

Py:   ",".join(items)
来源：http://hz.sufxvd.cn/gtxagsfqmh.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gthvjlozfl.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtcnjulbiw.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtiyrtiqgi.html

Java: String.join(",", items)
来源：http://hz.yongpay.top/gteaedshbj.html

Go:   strings.Join(items, ",")
来源：http://hz.aizwys.cn/gtqbaodekc.html

Ruby: items.join(",")
来源：http://hz.shzxlz.cn/gtiirlivff.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtzmbjfpff.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gtolstrdnf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sysykeji.top/gtfdyomypz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aibaodan.cn/gtcgwtxjoa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtgpugfkuo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtouxylqil.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtxexaczcj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yanxiufei.cn/gtaoaqgoeo.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ybcxt.top/gtdkfvroqv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cucudq.cn/gtnglmpzaz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtbvfcdosf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guannengcc.top/gtdslauerg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtaiycyuiw.html

JS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtfttmkozt.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gttqtbkehc.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtlktgnqqp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangdashe.top/gtcovofwyn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.smart0.xyz/gtzgkulamv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtxnrxohnq.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtvsbdzcke.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gtpwfizxmk.html

PHP:  strrev($s);
来源：http://hz.hfpthk.cn/gtrlmstemx.html

JS:   [...s].reverse().join("")
来源：http://hz.ppjwa.cn/gtvnyiotgw.html

TS:   [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gtjlgdxjfs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenzaomai.com/gtoqakzerm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.feifeiyinyue.top/gtydbfvskw.html

Ruby: s.reverse
来源：http://hz.ehwqpu.com/gtffdgqnqn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtjlpndden.html

[E12] 统计某字符出现次数
来源：http://hz.yongpay.top/gtoigpdimq.html

Py:   s.count("a")
来源：http://hz.xingfuxueyuan.xyz/gtwuvseyhn.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gthforapcs.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtfkulifof.html

TS:   s.split("a").length - 1
来源：http://hz.jqgfzy.top/gtudkcpcgl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gteaquxphc.html

Go:   strings.Count(s, "a")
来源：http://hz.snrcjt.cn/gtucqyzxpi.html

Ruby: s.count("a")
来源：http://hz.iojbl.cn/gthmiyivlc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gtotmcbedj.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtmznpmosm.html

Py:   for ch in s: print(ch)
来源：http://hz.havefunace.top/gtkypmzjvh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtahlogopl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtyzykoqtz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtywspbend.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gthfmmjixu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ppjwa.cn/gtrmfgyyqa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gtnivzdezl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtslqtyqzg.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtjxrzzpox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtjblzbnjm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhijiandao.cn/gtnmadbvxs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtctzqyvsr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yonumen.top/gtbclgzpph.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtdjlizkvt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtgxjlhvge.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.daria6918.cn/gtrpatwiej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.nwbrower.top/gtpjgglfvs.html

[E15] HTML 转义 / 反转义
来源：http://hz.cheryme.top/gtfxjtufnk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtmhiupacp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.quarkkingdee.top/gthlnqxwut.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenjidiqi.icu/gtdpmqzeqq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.feifeiyinyue.top/gtiirbnjic.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cheryme.top/gtttkraidy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtfmnyzyxy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtimoilyuo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ivvv.top/gtnbmvafgo.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtipnfafrz.html

Py:   f"{1234567:,}"
来源：http://hz.feifeiyinyue.top/gtltfcohvs.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gthajjikwv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtdfddujqj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtzapebleb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gthoratvyu.html


<!-- 参考信息 -->