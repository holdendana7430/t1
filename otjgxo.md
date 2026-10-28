代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj20258888.top/gtrhsnodwa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yongpay.top/gtzmturext.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zycfv.cn/gtttqrmkzl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yvedp.cn/gtoiqilqyx.html

[D11] 反转数组
来源：http://hz.ppjwa.cn/gtypsnjmgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnqzz.top/gtzqfmjswu.html

PHP:  array_reverse($arr);
来源：http://hz.ehwqpu.com/gtrkeivkkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.pengpengdd.cyou/gtbvlcenyu.html

TS:   [...arr].reverse();
来源：http://hz.yuxming.cn/gtkxopathl.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtzzdwlcep.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtrbtexkbt.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtftlusivr.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtencfuysf.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gtwcanxmbm.html

Py:   arr.index(x);  x in arr
来源：http://hz.gotoacloud.top/gtwdplpido.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtstxhmuha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtchnnwsgl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.birdmap.top/gtbmkcbgmp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gtmyrvnkxw.html

Go:   slices.Index(arr, x)
来源：http://hz.jinghuilouyu.cn/gtqihsltux.html

Ruby: arr.index(x)
来源：http://hz.svipenyu.cn/gtpfkudbia.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gthwvwtwkj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jyoumei.cn/gtygoooxbk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yonumen.top/gtgqsebtwc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtxkwbvysh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtlalyfcnt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtxrrdksof.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hywenlv.cn/gtgneapqdq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shuidangran.top/gtjoxcqtym.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.redwolf501.top/gtnknrvlxr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhiwuduotai.top/gtodvzoktu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gogol.net.cn/gtslftlbqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtprrivcax.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtmslwypgr.html

JS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gtkmplysui.html

TS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtsdwrsyhq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cheryme.top/gtqryokzdk.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtyghlucvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tian-w.cn/gtckjstohm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gtyqeenwtu.html

[D15] 去重
来源：http://hz.9152youxi.cn/gtwuvokidp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fzhhl.top/gtwgitqedy.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtjfmrdodn.html

JS:   [...new Set(arr)]
来源：http://hz.zycfv.cn/gtdqucrflu.html

TS:   [...new Set(arr)]
来源：http://hz.aibaodan.cn/gtwiienfez.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yonumen.top/gtzocgpbww.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtjsqbqczs.html

Ruby: arr.uniq
来源：http://hz.ivvv.top/gtfeozmmzj.html

C#:   list.Distinct().ToList()
来源：http://hz.yuxming.cn/gtuwxckxzu.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtfpmxcqkz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtdnnmwfpd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sweek.top/gtmdsusaac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtcdkqgbom.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtnmvqeuvm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtnvqllxsz.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtzyrkbhpv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinghuilouyu.cn/gtsaehnmtk.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtjxilxncj.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtcwegmqhz.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtobxarcve.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gttxnwcwlw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jianghu66.top/gtylylzhcu.html

TS:   Math.max(...arr);
来源：http://hz.ybcxt.top/gtbbivalmn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gtpvfrmyai.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.svipenyu.cn/gtrlaslpwt.html

Ruby: arr.max;  arr.min
来源：http://hz.ybcxt.top/gtyddfkkyb.html

C#:   list.Max();  list.Min()
来源：http://hz.zhixingplan.top/gtgfihjvzn.html

[D18] 扁平化嵌套数组
来源：http://hz.hnxiangtu.top/gtfdvmxdna.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cashguo.top/gtzkprhltb.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gtqvoiutwl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gtacgqiqdf.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtmojjwgcy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.haohaochexian.top/gtunmqgsqv.html

Go:   // 手写双层循环
来源：http://hz.gaohongyu789.top/gtnvlkysjh.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtdozdiprg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pengpengdd.cyou/gtqtihgqyw.html

[D19] 按字段分组
来源：http://hz.nwbrower.top/gtovlwtokw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtivjgguuj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhongyouzk.top/gthtqxdwmu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhengqikj.top/gtmvebhwgg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtxjqifpxp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yj20258888.top/gtytmvnsdw.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtraxxqeim.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtgcdtguht.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtyjnerazr.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtxorymkrx.html

Py:   Counter(arr)
来源：http://hz.9152youxi.cn/gtnfitjqjp.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtzlzzqdwf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtkwlouyza.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtnexdwcyz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenjidiqi.icu/gtgxgstiyh.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtqpwwdmvq.html

Ruby: arr.tally
来源：http://hz.nanxinkj.top/gtqoudkeve.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hywenlv.cn/gtbhhukxah.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gttahoioph.html

Py:   x in arr
来源：http://hz.jlsjyb.cn/gtgaqbboso.html

PHP:  in_array($x, $arr, true);
来源：http://hz.snrcjt.cn/gttsnpsgnj.html

JS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gttlseurio.html

TS:   arr.includes(x)
来源：http://hz.hammf.cn/gtbtidksvm.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtxfyntfxn.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtzqpizdyq.html

Ruby: arr.include?(x)
来源：http://hz.xinyue.icu/gtoytqxzps.html

C#:   list.Contains(x)
来源：http://hz.jinghuilouyu.cn/gtrhttyfnq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtmzqwsxik.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtjxgawcvo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.pengpengdd.cyou/gtxlxtgbhs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gttaqeuwzs.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gttgsfjykv.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gtvnvslouh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xinyue.icu/gtecdxrfor.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtxfpjhssk.html

C#:   new List<int>(list);
来源：http://hz.ybcxt.top/gturbbyvsf.html

[D23] reduce 累积计算
来源：http://hz.jyoumei.cn/gtyktzwilp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.0kj1m.cn/gtxdudplcp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pengpengdd.cyou/gtdrorqjbx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtvgrwigtz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtdbmbltsa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtafasoklo.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtzltbpqjg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guowangkeji.top/gtmjrkgrph.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sxryk.cn/gtiepflqln.html

[D24] 字典 / Map 基本操作
来源：http://hz.pycfn.com/gtpkiajpew.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtpngvqyfx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.pengpengdd.cyou/gtwmecyugj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yueranfly.top/gtaefztxyv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtjjzetfem.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gtbdueknyr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtlmoviqzn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtrztctixl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtnwqmyoai.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtubamodyq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtsnrnsojt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jiagoushi.top/gtmrpepbyo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtckfwjose.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tian-w.cn/gtpfxtyusa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtucgaulea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.meibo888.top/gtflqwwrvk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtryyboxss.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hongshengwenyu.top/gtcxcrueri.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtipqsvxsb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtbqfmqzow.html

PHP:  implode(", ", $arr);
来源：http://hz.zhixingplan.top/gtnswgelja.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtharhwmds.html

TS:   arr.join(", ")
来源：http://hz.c1oappe.top/gtqbavdkbu.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gtneccggct.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtwgwfbmtg.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtwbzpnvco.html

C#:   string.Join(", ", list)
来源：http://hz.kuanghao11.cn/gtuxvovopo.html

================================================================================
来源：http://hz.yangfankeji.com/gtlshywjwd.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtskhjkuwe.html

================================================================================
来源：http://hz.0kj1m.cn/gtcitfwjnj.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtoybadsuo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtpfwfoift.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tanke756.top/gtkjiblztb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtkxjdsqmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtcdxodgsz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sxryk.cn/gtensmdxwn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hfpthk.cn/gtqfjjnxpy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtxghxazmj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtyokeexxu.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gthtetdmjr.html

Py:   "ab" * 3
来源：http://hz.wangdashe.top/gtkpcwpobt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtifujlfxt.html

JS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtthpxbblx.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gtfzegpfnx.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtcaednguq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gtdshfbxla.html

Ruby: "ab" * 3
来源：http://hz.yj20258.top/gthxqggzyx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuanzx.com/gtivtvgaul.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gtspoeccbl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jyoumei.cn/gtwurytqbj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtbkzsrbmk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtudhonhgd.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gtshdmfvds.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtehpiqnyf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sysykeji.top/gtozikjmvc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtcvpwnacq.html

C#:   s.Substring(1, 3)
来源：http://hz.yvedp.cn/gtnxjzdeek.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gtrpcncvyl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinyuanbaomall.cn/gtpoionacz.html

PHP:  strpos($s, "x");
来源：http://hz.nanxinkj.top/gtvkmowzds.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtukdmkjmb.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtlosieyss.html

Java: s.indexOf("x")
来源：http://hz.gogol.net.cn/gtqsghnyxf.html

Go:   strings.Index(s, "x")
来源：http://hz.tian-w.cn/gtfhqubyho.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtcgulirzi.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtsunqhvlq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtaxbyfypc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtohhaifdn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtjvfpjdng.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtagrjtvsl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gogol.net.cn/gteglmhbmr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtnqnmzgqd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtbbrerbpi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fengsongda.top/gtjtjxaijc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yvedp.cn/gtddgtsfwy.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtkbmifhiz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuanzx.com/gtcfnpryks.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gotoacloud.top/gtcblulyxg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtzvhuskyl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtazzkdqsq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtxvpbjqbj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangshuangyany.cn/gtnxwwmsrc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pengpengdd.cyou/gtptqtiuxl.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtxnlzcowi.html

[E07] 按分隔符拆分
来源：http://hz.shzxlz.cn/gtjsfsceeg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtlualvegt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gttpbkihqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gtgbshpsis.html

TS:   s.split(",")
来源：http://hz.jiagoushi.top/gtaexldnih.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtmtoowevr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sysykeji.top/gtpwjquqnw.html

Ruby: s.split(",");  s.split
来源：http://hz.jyoumei.cn/gtkbgnjwia.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinqigufen.top/gtbaevbhml.html

[E08] 数组按分隔符合并
来源：http://hz.ehwqpu.com/gtwklrshnu.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtntmhdfkr.html

PHP:  implode(",", $items);
来源：http://hz.vqdsnc.cn/gtdxghryov.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtfdvglzfd.html

TS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtsiigcpmn.html

Java: String.join(",", items)
来源：http://hz.yj202588.top/gtbglvfxln.html

Go:   strings.Join(items, ",")
来源：http://hz.yuxming.cn/gtkwpwgsei.html

Ruby: items.join(",")
来源：http://hz.zhiwuduotai.top/gtsecavcng.html

C#:   string.Join(",", items)
来源：http://hz.bjfxy.top/gtvedqrzov.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtbfzidbhd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtjocoyicz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtgeoxubvd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gtrdqtqxwl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtjuhsjheu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtlxvzdcqa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtlivfbssf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtgvxoqlpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhijiandao.cn/gtvrvkhkxu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fzhhl.top/gtixyrnllt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtkcapkujg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxuanxn.top/gtllukclro.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtsmubuvso.html

TS:   "7".padStart(3, "0")
来源：http://hz.yueranfly.top/gtrtdtotpo.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtqguygfqo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtigasncwe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtzxszmdij.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dashuyun.cn/gtufzahugd.html

[E11] 反转字符串
来源：http://hz.wangshuangyany.cn/gtdjfsbsqt.html

Py:   s[::-1]
来源：http://hz.xuetiantiany.cn/gtdyxflxim.html

PHP:  strrev($s);
来源：http://hz.andypj.xyz/gtmvnjkcrn.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtryshwiox.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gttvztcblc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtgvljocpn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.fzhhl.top/gtisyqppln.html

Ruby: s.reverse
来源：http://hz.yangfankeji.com/gtibntjnfx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gthcvpsuyf.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gtchqnkyuj.html

Py:   s.count("a")
来源：http://hz.9152youxi.cn/gtqvxxddlp.html

PHP:  substr_count($s, "a");
来源：http://hz.fzhhl.top/gtkmzbebxx.html

JS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtqraubxpf.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtumoemzdn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtmektsnxn.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtbbtgfyxi.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtziryxjud.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtntdhztdr.html

[E13] 逐字符遍历
来源：http://hz.316326.xyz/gtxvcyyldf.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gthehougej.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dianchejie.cn/gthsdpfikr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtkizmsgvq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dashuyun.cn/gtngaasahc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gttspodsqt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtpvtntopk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtkjugnfdw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ybcxt.top/gtzlbauanv.html

[E14] URL 编码与 Base64
来源：http://hz.xingfuxueyuan.xyz/gtuflavegw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtvtaxxvim.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj202588.top/gtpuwfkpkg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ehwqpu.com/gtrgxoaace.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.redwolf501.top/gtowphwany.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtcwcuydfq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.c1oappe.top/gtocqvgwej.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yangfankeji.com/gtxceiyzgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtnknpglrw.html

[E15] HTML 转义 / 反转义
来源：http://hz.316326.xyz/gtwtigsrit.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtrgkcuzzr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guannengcc.top/gtejakytuo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtcgcxkorr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shangyingyoupin.top/gtlrsjqkdz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuetiantiany.cn/gtaopomfpq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtjvlaowuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yongpay.top/gtvzkzflho.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.iojbl.cn/gtqdhzuark.html

[E16] 数字千分位
来源：http://hz.cdnleiting.top/gtobmsjowo.html

Py:   f"{1234567:,}"
来源：http://hz.shangyingyoupin.top/gtdqcrgmri.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtpsxkyeuo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtowttkatf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtzkeooexp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258888.top/gttwdnxaqu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.guannengcc.top/gtalimdmet.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ywan-chungtsiang.top/gttyythkue.html

C#:   1234567.ToString("N0")
来源：http://hz.cheryme.top/gtbaxjmroo.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtmzapkstq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jlsjyb.cn/gtszsifcgt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258.top/gtraogqetj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnqzz.top/gtqzdlnucm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gttvuzfphj.html


<!-- 参考信息 -->