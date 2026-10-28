代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtqnshkffi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sweek.top/gthvwwhhdn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtiysyyvrs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtpbxeprhv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fengsongda.top/gtqxgpmpzf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gthjrdapkn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.mhx1999.top/gtehxdxbtm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gtodvqevmj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtstbgbnxu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jianghu66.top/gtaixvzzku.html

JS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gtrccohzjm.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtocliqxpr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cashguo.top/gtbwkdgatj.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtcuhyvzps.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinqigufen.top/gtlxmwgajq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aizwys.cn/gtzowfuzif.html

[D15] 去重
来源：http://hz.hywenlv.cn/gtjfwppzkx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gtxymjwiae.html

PHP:  array_unique($arr);
来源：http://hz.zhoulong.xyz/gtmvqbzrnn.html

JS:   [...new Set(arr)]
来源：http://hz.feifeiyinyue.top/gthdensekx.html

TS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtoxqrwsgj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hysaishi.cn/gtnbecxhjq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gtvgmfrtlh.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtcaphnjea.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gteoxatqbz.html

[D16] 求和与平均值
来源：http://hz.sysykeji.top/gtuqliaobh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtilhgedvy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtlvogsirz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gteizzrjhq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sxryk.cn/gtknsdefpy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.dashuyun.cn/gtctbjgsyg.html

Go:   // 手写循环累加
来源：http://hz.52xcode.cn/gtboxzlrgo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gthckmnciu.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gtltuvdfyo.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtfgdflibo.html

Py:   max(arr);  min(arr)
来源：http://hz.sxryk.cn/gtvdxmhaee.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtgbnpxrtx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtpaecyrzg.html

TS:   Math.max(...arr);
来源：http://hz.ehwqpu.com/gtfjvnryyy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gthincweqh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtbaokihot.html

Ruby: arr.max;  arr.min
来源：http://hz.ywan-chungtsiang.top/gtxetpnsey.html

C#:   list.Max();  list.Min()
来源：http://hz.shzxlz.cn/gthabpydwz.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigufen.top/gtciuznrvf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aizwys.cn/gtdxospbjb.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtbouqwave.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hywenlv.cn/gtrrilfoqp.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtrhnpnbna.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gtkvredhfg.html

Go:   // 手写双层循环
来源：http://hz.zycfv.cn/gtwrsetgjk.html

Ruby: nested.flatten
来源：http://hz.shangyingyoupin.top/gtclnyjoca.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cheryme.top/gtanirddmw.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gttoaimxvk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangshuangyany.cn/gtjskqhbjc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtiannunhb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.52xcode.cn/gtuydcassj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtsgvmrkdy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jianghu66.top/gtcmenchjx.html

Go:   // 手写 map[string][]T
来源：http://hz.wangdashe.top/gtnjtxxoxh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtejbnaprb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nwbrower.top/gtxmilbtpb.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtsstigamw.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtjlzwcvqp.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtsulzyyae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnxiangtu.top/gtzmixmwph.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cucudq.cn/gtknjicxuv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gtlgrhggmc.html

Go:   // 手写 map[T]int
来源：http://hz.aizwys.cn/gtidswzvct.html

Ruby: arr.tally
来源：http://hz.9152youxi.cn/gtuegaayiu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sufxvd.cn/gtpebbbjer.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtyxovkeam.html

Py:   x in arr
来源：http://hz.ivvv.top/gtaaoooock.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhaomingkeji.xyz/gtfojitvuy.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtnrbtkinl.html

TS:   arr.includes(x)
来源：http://hz.cashguo.top/gtobtcaron.html

Java: list.contains(x)
来源：http://hz.daria6918.cn/gtxgapnymz.html

Go:   slices.Contains(arr, x)
来源：http://hz.cucudq.cn/gtixksxaam.html

Ruby: arr.include?(x)
来源：http://hz.xziqi.cn/gtmwqsxrko.html

C#:   list.Contains(x)
来源：http://hz.shuidangran.top/gtepttwuut.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtvmjfjuoy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtekmbrbgr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinghuilouyu.cn/gtyejiythn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtopoleleq.html

TS:   [...arr];
来源：http://hz.nanxuanxn.top/gtwpeempzy.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtwslvzrvc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dianchejie.cn/gtkelegvbb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinyuanbaomall.cn/gtqsdzfpyw.html

C#:   new List<int>(list);
来源：http://hz.316326.xyz/gtzeqvxcte.html

[D23] reduce 累积计算
来源：http://hz.sweek.top/gtoweookdq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tanke756.top/gtdhbustpw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.redwolf501.top/gtwuqtnasn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtmuaifrbb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtkkhctqav.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtabvpiybz.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtjyseaydz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtldyoclgi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.52xcode.cn/gttzlbfefe.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtuzvfvvkz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtgvoqxoym.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhongyouzk.top/gthmqzuozs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ybcxt.top/gttoippxuv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtirhgnfcj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gthdqlasjm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangdashe.top/gtxkgmbeqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj202588.top/gtvurhegvv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangshuangyany.cn/gtswvqqhpq.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtkbhligku.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hywenlv.cn/gtirgpyzzd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.vqdsnc.cn/gtcgenkhij.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jyoumei.cn/gtwkoiwzcv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hywenlv.cn/gtndaqkwxo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtpgrvkpfb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtjnkmvasy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtwllyuljo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sysykeji.top/gtrapoglga.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtbggsiofd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gthtzcbfza.html

PHP:  implode(", ", $arr);
来源：http://hz.yongpay.top/gteapeccim.html

JS:   arr.join(", ")
来源：http://hz.yj202588.top/gteosaxiag.html

TS:   arr.join(", ")
来源：http://hz.yueranfly.top/gtzwwjtppw.html

Java: String.join(", ", list)
来源：http://hz.ydjk.org.cn/gtxnsiajfl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtcukfgmgy.html

Ruby: arr.join(", ")
来源：http://hz.ydzc1.top/gtoobnktxy.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gtsfmabtyi.html

================================================================================
来源：http://hz.nwbrower.top/gtlxecczcd.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gthgbhmorm.html

================================================================================
来源：http://hz.yonumen.top/gtnoevfqcr.html

[E01] 拼接字符串
来源：http://hz.jianghu66.top/gtntjcpvap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtsgefstkt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sysykeji.top/gtaicvkiqq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtkhwxgohc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtyqyuevkk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtjxqeelcj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtnhxxtmwn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.svipenyu.cn/gtkljdrtjk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtqzazzukg.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtjmmhbrrc.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtblbkbotn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.snrcjt.cn/gtnaqqkdvg.html

JS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtjzdqhszv.html

TS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gthptkjyll.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtcfzjnkmi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtfbmgafyw.html

Ruby: "ab" * 3
来源：http://hz.aizwys.cn/gtgwuhbcmr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gtdhnxqfui.html

[E03] 截取子串
来源：http://hz.yuanzhike.top/gtisaspmhg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtpewkdhic.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yanxiufei.cn/gtstycxzbc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtpdykmydh.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtjipotfpx.html

Java: s.substring(1, 4)
来源：http://hz.cheryme.top/gtzvmcsnce.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.vqdsnc.cn/gtevimnzvp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuxming.cn/gtltesfqdh.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtotdcdybe.html

[E04] 查找子串位置
来源：http://hz.tian-w.cn/gtuyisoqnr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtfjjwqogk.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtgzzkjvrd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shangyingyoupin.top/gtzftxbkvq.html

TS:   s.indexOf("x")
来源：http://hz.hfpthk.cn/gtigphjlwz.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtzsarjlzn.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtlcmummtk.html

Ruby: s.index("x")
来源：http://hz.cdnleiting.top/gtwdgvrtpi.html

C#:   s.IndexOf("x")
来源：http://hz.shangyingyoupin.top/gtnugiglix.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.pycfn.com/gtjctmbtqa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jyoumei.cn/gtsqnjxbrs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtyiifrcmm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtcyapatrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtgnrbhmad.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gtkwxpawcq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.c1oappe.top/gtzhyaykmm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ivvv.top/gtodippgtf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gzhubu.top/gtelqybmsq.html

[E06] 替换子串
来源：http://hz.hysaishi.cn/gtmpqodcmg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuanzx.com/gtzbicrhye.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxinkj.top/gtmgoqvcoz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtwmdlakic.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gticucnbuh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtlxpvhyhd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtaitmnxqp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtnkkthfsz.html

C#:   s.Replace("a", "b")
来源：http://hz.yj20258.top/gtxgzwmgdv.html

[E07] 按分隔符拆分
来源：http://hz.chenjidiqi.icu/gtzzvaorqp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtleagjree.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydjk.org.cn/gtvnxaxauz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gaohongyu789.top/gtylvmhxnd.html

TS:   s.split(",")
来源：http://hz.jiagoushi.top/gtuwaiqdel.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yangfankeji.com/gtuzlhjmgq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.redwolf501.top/gtszxajhej.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtgzdygaxt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gtfkwkxccg.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gteucekfzu.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gtwwduzusd.html

PHP:  implode(",", $items);
来源：http://hz.daxiang520.top/gtvzdubalz.html

JS:   items.join(",")
来源：http://hz.ybcxt.top/gthpcpyblp.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtyfpuemjg.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtnnwmthjn.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtprgdnlgn.html

Ruby: items.join(",")
来源：http://hz.zhongyouzk.top/gtwgcvksbl.html

C#:   string.Join(",", items)
来源：http://hz.nanxinkj.top/gtsuakginf.html

[E09] 去除所有空白字符
来源：http://hz.sufxvd.cn/gtfeegcfin.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtqruynqym.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtrnfofeqm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtqucpgetx.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.birdmap.top/gtwltbyprj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuxming.cn/gtsxndjqdj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtvkpbiuik.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtiwhovjsx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.snrcjt.cn/gtyspybufu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinghuilouyu.cn/gthokuzkwe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtibhfjawp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtamzdtcgv.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhixingplan.top/gtzazlkszv.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtyllnzidt.html

Java: String.format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtnstrohqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.andypj.xyz/gtwpmllmzo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gtgczykzec.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtchpemyjr.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gttiyxakws.html

Py:   s[::-1]
来源：http://hz.9152youxi.cn/gtkmjrcgkf.html

PHP:  strrev($s);
来源：http://hz.yj202588.top/gtwfzwurrq.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtoxhkuwwl.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtzzttqydv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gaohongyu789.top/gtvtdvvtdz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtibwhbzgs.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gthdlxjhay.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtmttfzgob.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtvzxzqtfr.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtkitvqafi.html

PHP:  substr_count($s, "a");
来源：http://hz.yj20258888.top/gtfwjtcpdy.html

JS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtsgwqtxox.html

TS:   s.split("a").length - 1
来源：http://hz.wangdashe.top/gtnqkyatte.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtjjkhjnns.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtzlmslcmm.html

Ruby: s.count("a")
来源：http://hz.zdqjudy.top/gtfttachnw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.quarkkingdee.top/gtttbnfrqk.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gtwhxzhhxd.html

Py:   for ch in s: print(ch)
来源：http://hz.zdqjudy.top/gtxipajkem.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigufen.top/gtqtebeerp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtvkzpsdic.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sysykeji.top/gtaemeihzi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuanzx.com/gtnurnbgzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jianghu66.top/gtmdoosxpb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhoulong.xyz/gtlzrweysw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangdashe.top/gtvzolwpaj.html

[E14] URL 编码与 Base64
来源：http://hz.guannengcc.top/gtkvfocmri.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.vqdsnc.cn/gtyjwpvotb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtavnjrcun.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.dianchejie.cn/gtpozcpxtt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ppjwa.cn/gtgpazosri.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtdqdfksal.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtkznqdehf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gtaxbsymvu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fengsongda.top/gtrsjmnyll.html

[E15] HTML 转义 / 反转义
来源：http://hz.shangyingyoupin.top/gtcejamxgw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jianghu66.top/gtuvmlhvum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zdqjudy.top/gttpsmxpqy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jianghu66.top/gtjxnwamey.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gthwdbersn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxuanxn.top/gtcaeryiyu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.svipenyu.cn/gtgvskqiki.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.mhx1999.top/gtbcusfxoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtqnmtyyva.html

[E16] 数字千分位
来源：http://hz.havefunace.top/gtuzqyomtc.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtkgnmqunx.html

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtlrdeapus.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtjyngyoye.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinyuanbaomall.cn/gtorycqdad.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtngsufgyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtlbijqewp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.9152youxi.cn/gtznmeeowm.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gtjyescfqi.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtssehbweu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuetiantiany.cn/gtuaqivxey.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtyeomlrhx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtnojmwxcb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtvzmclsfv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cashguo.top/gtfaniamak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtmfilqgmd.html

Ruby: s.capitalize
来源：http://hz.ehwqpu.com/gtyywwfdnd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.svipenyu.cn/gtptwmamyq.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtiwdtvbwe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cdnleiting.top/gtbpcmvgbj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cheryme.top/gtejjkglbz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtxfzzhvwv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtmcbqicsm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtrwwkytfs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.0kj1m.cn/gthuuepevh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gtyqioepgw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtjtmlwybs.html

[E19] 多行文本按行拆分
来源：http://hz.jlsjyb.cn/gtfildgrro.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtfjtzxtdy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hysaishi.cn/gtqusqamed.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtmofjouqc.html

TS:   s.split(/\r?\n/)
来源：http://hz.dashuyun.cn/gtlspinytz.html

Java: s.lines().toList()
来源：http://hz.guannengcc.top/gtvajqnhlg.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtlwzqwuxu.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtbnqvcfvn.html

C#:   s.Split('\n')
来源：http://hz.ydjk.org.cn/gtzbeknskf.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gthpfkmvpr.html

Py:   if not s:
来源：http://hz.sweek.top/gtidjfnxjy.html


<!-- 参考信息 -->