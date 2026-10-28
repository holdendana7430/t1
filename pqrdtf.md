代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.52xcode.cn/gtrxajmcsh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtuiymmkxt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtqtisjuss.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtqfspznfj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cheryme.top/gtyprzwdbw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hysaishi.cn/gtcgjimvtz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtpukxkhdi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtpmqlvlkc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangshuangyany.cn/gtfiuxacng.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtgmroaypq.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtcxtspbpv.html

TS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtnszchdmy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtuehenbwe.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtovnnqdfe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtqnoeplzh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhongyouzk.top/gtflswegzo.html

[D15] 去重
来源：http://hz.xylfe.cn/gtjjexfxrv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnqzz.top/gtocqghgwr.html

PHP:  array_unique($arr);
来源：http://hz.xuanzx.com/gtsnaiekdv.html

JS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtwlfeurnj.html

TS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtkjnhsyzx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtwgjstchc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhongyouzk.top/gtrhdhlgwu.html

Ruby: arr.uniq
来源：http://hz.feifeiyinyue.top/gtuybzyugq.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtrqxsykvh.html

[D16] 求和与平均值
来源：http://hz.xziqi.cn/gtgnwyxzbe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sweek.top/gtlgqbknyj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtaktdrrwa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtpksswpui.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhixingplan.top/gtpourgehp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtjcktjubb.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtsqlwwfcg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtfygeaklc.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtuibzkjgp.html

[D17] 最大值与最小值
来源：http://hz.xingfuxueyuan.xyz/gtramfaurt.html

Py:   max(arr);  min(arr)
来源：http://hz.yonumen.top/gtxdetdboj.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenlongwang.top/gtvoxrjyar.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gteghkauow.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtvqyuwukb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhiwuduotai.top/gtfkthyfrt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gtpqntizhy.html

Ruby: arr.max;  arr.min
来源：http://hz.daxiang520.top/gtqblpdgbm.html

C#:   list.Max();  list.Min()
来源：http://hz.havefunace.top/gtgdlujpog.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtzufvrqly.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtrjtoihfg.html

PHP:  array_merge(...$nested);
来源：http://hz.ivvv.top/gtotldmamm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtkwvnhwro.html

TS:   nested.flat();
来源：http://hz.andypj.xyz/gtjyqgxegb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxuanxn.top/gtjjocsdog.html

Go:   // 手写双层循环
来源：http://hz.jiagoushi.top/gtlusnwlsr.html

Ruby: nested.flatten
来源：http://hz.xziqi.cn/gtljpvfkyd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gteznkqyvv.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtmsytyghw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zycfv.cn/gtltozflsx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtouvrwcvl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtclfibruc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtgqwxwblq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shzxlz.cn/gtujuaciks.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtoalkebtx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.316326.xyz/gtdobesupw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xylfe.cn/gtoeoytotr.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gthmfzzvup.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gthtwjdusa.html

PHP:  array_count_values($arr);
来源：http://hz.hnxiangtu.top/gtyggqedom.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinyuanbaomall.cn/gtauwltvxt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtusklphtc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtbkuqatms.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtkbhixruf.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtptmnnnch.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gogol.net.cn/gtoxxlrpic.html

[D21] 判断是否包含某元素
来源：http://hz.hongshengwenyu.top/gtvhlrgfwc.html

Py:   x in arr
来源：http://hz.jqgfzy.top/gtisjhcajk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.fengsongda.top/gtorocjmiv.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtzdnnklvd.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtvjetwxzn.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtoamnjrdq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yvedp.cn/gtrvkrrell.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtcxczcylg.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtcixgnsnp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gaohongyu789.top/gtiabqfwrm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yonumen.top/gtmznxcgzh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtkrbfajbf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zdqjudy.top/gtjwbrpxtx.html

TS:   [...arr];
来源：http://hz.wangshuangyany.cn/gtseitkksu.html

Java: new ArrayList<>(list);
来源：http://hz.hfpthk.cn/gtbjrvyzpj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtwqxxzgfb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.iojbl.cn/gttbcqqxhk.html

C#:   new List<int>(list);
来源：http://hz.xuetiantiany.cn/gtvwljpozv.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtletbcnhr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangtech.top/gtfzwmsoaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenzaomai.com/gtbdbgwhws.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gzhubu.top/gtomjggeox.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtrvtlxlya.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shzxlz.cn/gttqmrbhuu.html

Go:   // 手写循环
来源：http://hz.tanke756.top/gthsizvukt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtpcrrjlda.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtphvhubwx.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtkrrujhmc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sysykeji.top/gtrhxkjuqu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgufenzy.top/gtwbzafczv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.52xcode.cn/gtkqwllxeq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ivvv.top/gtjblcslzt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtlfbtzyhf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinyuanbaomall.cn/gtdxqteiqo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tanke756.top/gtawuhikul.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pengpengdd.cyou/gteqysshcb.html

[D25] Set 集合去重与交并差
来源：http://hz.chenzaomai.com/gttrxjmcvo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cashguo.top/gtxmzqmbsd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hywenlv.cn/gtnfcftvsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtvekjfjgv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aibaodan.cn/gthhjizcie.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gthezzvfoj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtoipdquii.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gtooskncrg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yongpay.top/gtjpumcazu.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtopcsizua.html

Py:   ", ".join(map(str, arr))
来源：http://hz.iojbl.cn/gtbdlqpzie.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gthoenccer.html

JS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtpvukrfum.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtibzxqhal.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtzpzxrncp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtmljicrni.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtxdzshtkc.html

C#:   string.Join(", ", list)
来源：http://hz.jianghu66.top/gtfjijfoyk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpqshomtz.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtjyznajgt.html

================================================================================
来源：http://hz.jyoumei.cn/gthmrrkoyr.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtwwovnnyp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtkqqkqole.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258.top/gtstaupdgn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtmyhlfijt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtmttrqojf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtqkmgagcu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.guannengcc.top/gtayjppbww.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenjidiqi.icu/gtaekjqegp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtnejujmiv.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gteccqpgtp.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gteaxvxaev.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhongyouzk.top/gthmcohehm.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtotagkwyn.html

TS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtajbkpqdv.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtwoxxstac.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jyoumei.cn/gtglttvkfj.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtqnkplqch.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cheryme.top/gthpszaxnp.html

[E03] 截取子串
来源：http://hz.zhijiandao.cn/gtzjloezzi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sxryk.cn/gtruvhzxyi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtiqjvusox.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenjidiqi.icu/gtzmrohtse.html

TS:   s.slice(1, 4)
来源：http://hz.gaohongyu789.top/gtxefvjtiy.html

Java: s.substring(1, 4)
来源：http://hz.redwolf501.top/gtwkcoxomb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ivvv.top/gtzscmxamf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jqgfzy.top/gtugbjfwzr.html

C#:   s.Substring(1, 3)
来源：http://hz.pengpengdd.cyou/gtignbuqua.html

[E04] 查找子串位置
来源：http://hz.hysaishi.cn/gttwjqaidj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtdeevmgyy.html

PHP:  strpos($s, "x");
来源：http://hz.xinyue.icu/gtojsorbcu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtwonmskhx.html

TS:   s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtnlogelhc.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtbkhmmoly.html

Go:   strings.Index(s, "x")
来源：http://hz.yj20258888.top/gtqzcgwcqu.html

Ruby: s.index("x")
来源：http://hz.hysaishi.cn/gtzegvlwzp.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtcxvbruxb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jlsjyb.cn/gttsknveva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.iojbl.cn/gtxzzqwqmx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yueranfly.top/gtxceeofbj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gtraosatne.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.feifeiyinyue.top/gtivbycsst.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtpwjtwqwz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.svipenyu.cn/gtnizkmogu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cashguo.top/gtgcuxomzt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtcylznvbd.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtvkogssdf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtgekhdtzi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinyuanbaomall.cn/gtnaozrefv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtpqclnbat.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtrsckvwsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gtkyjepygr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ppjwa.cn/gtxhsiuwbc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258888.top/gtikvawwjn.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtqlinshte.html

[E07] 按分隔符拆分
来源：http://hz.316326.xyz/gtzunytjfm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hysaishi.cn/gtessmqxlx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtmaazgtpe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtdntblyxm.html

TS:   s.split(",")
来源：http://hz.xuetiantiany.cn/gtxrdykqsq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtjhoumhjp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gteejdoevn.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtbuccgqkr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtsonhzdxr.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtgxefezjv.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtlyvtkmuw.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtbdikujwu.html

JS:   items.join(",")
来源：http://hz.tanke756.top/gtnmtxpeiy.html

TS:   items.join(",")
来源：http://hz.ybcxt.top/gtiffovjph.html

Java: String.join(",", items)
来源：http://hz.316326.xyz/gtvrhqqszr.html

Go:   strings.Join(items, ",")
来源：http://hz.dashuyun.cn/gtiydkvpky.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtztmsbjuv.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtxthbxipg.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtmaqlifhv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tanke756.top/gtuuvxwbsk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtrzeunnpz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj202588.top/gthxtjkolr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gthbivbqll.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtvefuzbya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtgyoxdfao.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cdnleiting.top/gtjsugxagx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtqdayyctc.html

[E10] 左侧补零 / 定长填充
来源：http://hz.redwolf501.top/gtgfnlmxan.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.feifeiyinyue.top/gtbxdvkehk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtglthshuw.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtlvyljuzo.html

TS:   "7".padStart(3, "0")
来源：http://hz.havefunace.top/gtqadslgwe.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtyvpbsmtf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tian-w.cn/gtmmvhpnmg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xziqi.cn/gtvteznekb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtkqrwulft.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtbgpldgwm.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtinpwpinr.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtjfwxqpxw.html

JS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtbogolvjf.html

TS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtbsgjxsyg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.haohaochexian.top/gtsxunhteq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gttqigjchd.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtypjnraug.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtraaqecsw.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gtvzjrmnql.html

Py:   s.count("a")
来源：http://hz.ydjk.org.cn/gtzjbqjgzf.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtisunhods.html

JS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtnwzfplct.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtsnhieack.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtzkesdjmh.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtlrxkinta.html

Ruby: s.count("a")
来源：http://hz.wangdashe.top/gtlmeqslzf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ybcxt.top/gtkfkneefp.html

[E13] 逐字符遍历
来源：http://hz.hysaishi.cn/gtxwrosthg.html

Py:   for ch in s: print(ch)
来源：http://hz.yanxiufei.cn/gtciosojue.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtnkywripq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtxnafyhua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.havefunace.top/gtgdhrdgch.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sweek.top/gttwtyibet.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenlongwang.top/gtuoipcajt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gthgnhwwlt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhongyouzk.top/gtppqqsomm.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtojxsunta.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtlztsmhal.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtgaemziua.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenjidiqi.icu/gtcsxwwuan.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ybcxt.top/gtzwubamed.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinyuanbaomall.cn/gtnavbudnx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtaqorkyih.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtiuttxkpq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtfndspyol.html

[E15] HTML 转义 / 反转义
来源：http://hz.gogol.net.cn/gtdbdqnnln.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtegcmfrwt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jlsjyb.cn/gtgxcdeogx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtwuukljde.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuxming.cn/gtsghfwxhx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtmnczhdez.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yonumen.top/gtlzvtodwp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ydzc1.top/gtecyjidkk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtslcjvhiu.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtuxfsihtc.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gtspfuhwyk.html

PHP:  number_format(1234567);
来源：http://hz.yuxming.cn/gtgqlqaznf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtyfpajpyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtayuionii.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtesbijtga.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtjxtutbei.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtozpfhmhg.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gtzsxyxalu.html

[E17] 首字母大写
来源：http://hz.ppjwa.cn/gtehkxcpug.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ybcxt.top/gtpimisftd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtnrvlvbhs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtkamhiiaj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtdydfaevs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtghgajvmz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gaohongyu789.top/gtjequuwfq.html

Ruby: s.capitalize
来源：http://hz.havefunace.top/gtiffcgrgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtyvpgihwy.html

[E18] 模板占位符替换
来源：http://hz.meibo888.top/gtqtunlrvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gtulcvuuzf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.havefunace.top/gtuoubabdb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtmyzavivp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtwoiqovgi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtaikiwkmd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pengpengdd.cyou/gtrnquhkda.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtnpmmunxi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.c1oappe.top/gtmkygynls.html

[E19] 多行文本按行拆分
来源：http://hz.dianchejie.cn/gtudzvtybn.html

Py:   s.splitlines()
来源：http://hz.jqgfzy.top/gtstiucdhq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.9152youxi.cn/gthjugdsld.html

JS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtecuccyke.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhixingplan.top/gtkzuarmyk.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtbvdkgvhr.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtrzsaafoq.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtqjblweeh.html

C#:   s.Split('\n')
来源：http://hz.cashguo.top/gtvzrqisjn.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtovusihiu.html

Py:   if not s:
来源：http://hz.hywenlv.cn/gtffeyuqxg.html


<!-- 参考信息 -->