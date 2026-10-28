代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtunpfludh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinghuilouyu.cn/gttwksojbo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtsogwcdif.html

[D14] 映射转换（每个元素变形）
来源：http://hz.havefunace.top/gtzmkxlonz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sufxvd.cn/gtxbojbqlh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtgbnduros.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtagsucxcc.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtwofpmita.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtxmmxqgdm.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gtotbkpiht.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhoulong.xyz/gtolzrqxxx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtnrwosfnq.html

[D15] 去重
来源：http://hz.jinqigufen.top/gtvmtzeabo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhaomingkeji.xyz/gtbhkmpwro.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtcolwygbf.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtpasiusfa.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtcnawpewj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shzxlz.cn/gtwzflzzbx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtzrufmicl.html

Ruby: arr.uniq
来源：http://hz.zdqjudy.top/gtrtdsfgsp.html

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtlibagtui.html

[D16] 求和与平均值
来源：http://hz.haohaochexian.top/gtrdxbwkvb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shangyingyoupin.top/gtxtdqsank.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhongyouzk.top/gtuaozlqza.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtezfujqdt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jianghu66.top/gtqgohwfdh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtwiaalckl.html

Go:   // 手写循环累加
来源：http://hz.yueranfly.top/gtqtpksuiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shanyushiyangkeji.top/gtmyworcfm.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtbavbxhgo.html

[D17] 最大值与最小值
来源：http://hz.yonumen.top/gtuvkthmzo.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtpnlirvpd.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtrcwlkzga.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sysykeji.top/gtuciiytwo.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtfadhdfwd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.kuanghao11.cn/gtwqpkxdsd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtofdnuxfi.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtnjdnjfud.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gthflmevmz.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtvwukyicv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtjiqgmdlw.html

PHP:  array_merge(...$nested);
来源：http://hz.daxiang520.top/gtrbtiptgz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ppjwa.cn/gtnxatcjry.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtgmsiucps.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtjolhkncx.html

Go:   // 手写双层循环
来源：http://hz.cdnleiting.top/gtmxdoyzei.html

Ruby: nested.flatten
来源：http://hz.tian-w.cn/gtiqubrjcz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtjpjybndu.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtfmtnkrxu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtcexakdrv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtphfogdbu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhiwuduotai.top/gtfyrlvbnm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtskkoxdrs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangshuangyany.cn/gtuydqudfi.html

Go:   // 手写 map[string][]T
来源：http://hz.yangfankeji.com/gtvdvfzfvh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtnvfadffm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.snrcjt.cn/gtevhgjuam.html

[D20] 统计每个元素出现次数
来源：http://hz.nanxinkj.top/gtcbshzmoc.html

Py:   Counter(arr)
来源：http://hz.daxiang520.top/gtjjdkbsis.html

PHP:  array_count_values($arr);
来源：http://hz.pycfn.com/gtsxgqslil.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gteklzyxga.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtvadnrkun.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.birdmap.top/gtnfrafbta.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtbhxjkroi.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtzgaznbtq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hongshengwenyu.top/gtuhqmgvsl.html

[D21] 判断是否包含某元素
来源：http://hz.sweek.top/gtmmeboffv.html

Py:   x in arr
来源：http://hz.zhijiandao.cn/gtvygjhgwl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtcrbulfpp.html

JS:   arr.includes(x)
来源：http://hz.andypj.xyz/gtuaytdgox.html

TS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtkjieuetl.html

Java: list.contains(x)
来源：http://hz.iojbl.cn/gtgnjdumct.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtxxlifnzb.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtkfqpwucs.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtkwjkjfkh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtqotfxgcz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gtfyrejfff.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtaozgrwmp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.0kj1m.cn/gtkifurphf.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gturkmzigm.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtqaewnahf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtyvxangib.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtnkukiooo.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gtvlvnkplm.html

[D23] reduce 累积计算
来源：http://hz.wangdashe.top/gtuikugxhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtoejpmxhd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.quarkkingdee.top/gtwcmxsqpc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtpnjzklkl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtcqhxsjdw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtoiyabixf.html

Go:   // 手写循环
来源：http://hz.iojbl.cn/gtzzlsgery.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtolbqrhwt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtfofrqsfb.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gthppgeogo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtqustbhys.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cdnleiting.top/gtyjwzxanw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gotoacloud.top/gtpdiikvss.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guannengcc.top/gtmzmczapl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtxqrighof.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.tian-w.cn/gthfwjtubk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gttachwsmf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtkidjliqn.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtgqlcuplw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtftjrkjaw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtrjpvfyph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtuapzgtob.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gtzvuaiato.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shuidangran.top/gtdpnerxxd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtqyjinqzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ywan-chungtsiang.top/gteykhllbf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ywan-chungtsiang.top/gtqopdylyy.html

[D26] 数组转字符串
来源：http://hz.zhijiandao.cn/gtrkgvgdom.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtqwiybndd.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gteefuitrs.html

JS:   arr.join(", ")
来源：http://hz.316326.xyz/gtfjmebbnx.html

TS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtjqgwwhbl.html

Java: String.join(", ", list)
来源：http://hz.zhengqikj.top/gtveiakckr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.52xcode.cn/gtowlkgupb.html

Ruby: arr.join(", ")
来源：http://hz.andypj.xyz/gtmuctisup.html

C#:   string.Join(", ", list)
来源：http://hz.daria6918.cn/gtaubejynh.html

================================================================================
来源：http://hz.andypj.xyz/gtqbgiuupi.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gtgqhxpnot.html

================================================================================
来源：http://hz.sysykeji.top/gtnomkbwxu.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gtepbgqkgk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yvedp.cn/gtdwnxylvq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtucvprtio.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtlkzmswso.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtspweofur.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gtvgwzaote.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangshuangyany.cn/gtwzlixgns.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtvbjpwdhe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtwcsrhwst.html

[E02] 重复字符串
来源：http://hz.ivvv.top/gtjywateew.html

Py:   "ab" * 3
来源：http://hz.yonumen.top/gtvicqxyot.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hywenlv.cn/gtlbjncmqt.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtkliqkgxu.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtfjygimqi.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtymeesdcp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.quarkkingdee.top/gtxbwfehnm.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gteeetmvyc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtvpfnlgiz.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtbxwgcmgq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.redwolf501.top/gtugcbnzyj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtqmqsdelx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtwwfbtwsz.html

TS:   s.slice(1, 4)
来源：http://hz.chenlongwang.top/gtzcmjkpye.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtpnncptyo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhaomingkeji.xyz/gtzrskzfgk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhaomingkeji.xyz/gtwolqqaub.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtzlacbmds.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtfuiaaujk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xylfe.cn/gtdkiciccz.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtfwxggzlw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yonumen.top/gtqeorocpi.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gthrdvyyls.html

Java: s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtdsgftaik.html

Go:   strings.Index(s, "x")
来源：http://hz.yonumen.top/gtpxggdxmw.html

Ruby: s.index("x")
来源：http://hz.xylfe.cn/gtcqakqthw.html

C#:   s.IndexOf("x")
来源：http://hz.gotoacloud.top/gtltkexkqq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtklhoxjue.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dashuyun.cn/gtwybzrgcw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydzc1.top/gtnsbybsnw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtwdptdfvc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtddmcogaw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zycfv.cn/gtqvmrkbla.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.bjfxy.top/gtsatzrpay.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gtvyhacgks.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtwmtozunb.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtazmisdii.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgfzy.top/gtkgrgjjty.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtebygyovs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtqbsqvuiw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtqmwarzjr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gtsukiapbp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gogol.net.cn/gtdimriihb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.52xcode.cn/gttlsxcbcf.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtvxcfrvoz.html

[E07] 按分隔符拆分
来源：http://hz.ydzc1.top/gticwmhfnx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.meibo888.top/gtelgpzylq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xinyue.icu/gteejimqkj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtmzicwzzh.html

TS:   s.split(",")
来源：http://hz.shanyushiyangkeji.top/gtzcyokfek.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinyuanbaomall.cn/gtniqvzenj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhixingplan.top/gttxvcpitw.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtxsmzdphh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sufxvd.cn/gtqlqlkowe.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtajshtyfm.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtxlibgqgi.html

PHP:  implode(",", $items);
来源：http://hz.tianlin.xyz/gtyndmvuzs.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtqteufbih.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtjxcsqjkz.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gtamzhjtim.html

Go:   strings.Join(items, ",")
来源：http://hz.gotoacloud.top/gtgbcxnyit.html

Ruby: items.join(",")
来源：http://hz.feifeiyinyue.top/gtxetwmecg.html

C#:   string.Join(",", items)
来源：http://hz.nanxinkj.top/gtbanxlzmg.html

[E09] 去除所有空白字符
来源：http://hz.fzhhl.top/gtvczmteup.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtmmratrxy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtztxaaate.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtpmarakfb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtmhzctnwu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtoefciosh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.quarkkingdee.top/gtflxfrmjz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtnzdrlbvm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtduyqrmbs.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yvedp.cn/gtkjbelcvf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtlkqnieck.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zdqjudy.top/gtozhtdltc.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtwhvrwuve.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtmjmbrcia.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtogzeekii.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yonumen.top/gtjzrzlxoz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtjvfcupse.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinqigfzy.top/gtijuosjhg.html

[E11] 反转字符串
来源：http://hz.wangdashe.top/gtvqogying.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtufrxdpqx.html

PHP:  strrev($s);
来源：http://hz.yanxiufei.cn/gtnrlzatja.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtvojhxmuo.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtkuxsbjck.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gteihlfxny.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtqlzuixmn.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtfcwvdlnj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtjxatrylp.html

[E12] 统计某字符出现次数
来源：http://hz.yj20258.top/gtecpdecdp.html

Py:   s.count("a")
来源：http://hz.mhx1999.top/gtqnukafdp.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtiaswkqvw.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtuqpplyys.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtglnkuecd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.9152youxi.cn/gtkkdbwwev.html

Go:   strings.Count(s, "a")
来源：http://hz.0kj1m.cn/gtxslcxbnd.html

Ruby: s.count("a")
来源：http://hz.ydzc1.top/gtufuewfdc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gthifyrekw.html

[E13] 逐字符遍历
来源：http://hz.yj202588.top/gtqwvdubgz.html

Py:   for ch in s: print(ch)
来源：http://hz.xylfe.cn/gtkxihkovb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtovmbcxtd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtsnramiel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtbzuhglgz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtxmcdhvvf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtoqrnfkxz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nwbrower.top/gtkzvxdupp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtcshioezl.html

[E14] URL 编码与 Base64
来源：http://hz.yanxiufei.cn/gtyiiaqtvq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.52xcode.cn/gtohfcixfg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtayvkjdxp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnxiangtu.top/gttmmbctkq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtjegpnrpq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtvxworrqk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtxjamppqo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenzaomai.com/gthxbyxjck.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yangfankeji.com/gtscurcxor.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtveyvveis.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuxming.cn/gtwjllcjsb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhiwuduotai.top/gtxtokrckn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtvsacxyod.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtbjyonlzt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtnkhuakvq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hnqzz.top/gtrlwxcgsg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gtilzcedvp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.tianlin.xyz/gtfuqjytuq.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtfdnqdbso.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258888.top/gtjbptxfjv.html

PHP:  number_format(1234567);
来源：http://hz.jinqigfzy.top/gtogmdgxqn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtlmqvxpex.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtvezshybk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgufenzy.top/gtlktutcju.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtglbblmsr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gtrlyjwrfd.html

C#:   1234567.ToString("N0")
来源：http://hz.daria6918.cn/gtvgrgdaos.html

[E17] 首字母大写
来源：http://hz.jinqigufen.top/gtncyergps.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtnkincyri.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhengqikj.top/gtufsgqbin.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtzxxqxpvk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gthiooaibv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zdqjudy.top/gtlhmxmlyi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cashguo.top/gtzeztvgsl.html

Ruby: s.capitalize
来源：http://hz.gotoacloud.top/gtllhqacqj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangkeji.top/gtipohlzvh.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gtzlziyaqh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yangfankeji.com/gtveahegbu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fengsongda.top/gtnvazjmbh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.wangshuangyany.cn/gtwlileehd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hammf.cn/gthkpwfztq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gttfyqtglv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenzaomai.com/gteduypzpp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtjjzeixnk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hammf.cn/gtnjsimbmi.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtkagjotrj.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gthnjixtil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gaohongyu789.top/gtdhtmcvpl.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtgvksdpkd.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtqpwbucvr.html

Java: s.lines().toList()
来源：http://hz.tianlin.xyz/gtyblhptoj.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtcwigwkwy.html

Ruby: s.lines
来源：http://hz.svipenyu.cn/gtpvxmzjop.html

C#:   s.Split('\n')
来源：http://hz.iojbl.cn/gtblbtxgsh.html

[E20] 判断字符串是否为空
来源：http://hz.nanxuanxn.top/gtbszgsmnd.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtyurzvcfx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.quarkkingdee.top/gtzywyubsj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.iojbl.cn/gtaiirrssv.html

TS:   if (s === "") {}
来源：http://hz.xuanzx.com/gtsullzznr.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtiqqoyxjc.html


<!-- 参考信息 -->