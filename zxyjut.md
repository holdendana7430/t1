代发 wailian999

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gthnbjqxwe.html

C#:   list.IndexOf(x);
来源：http://hz.jinyuanbaomall.cn/gtajqkkcjc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gtazkmdzgl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtlpgvcfao.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yvedp.cn/gtqwndpvtj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtuargwato.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtydsnwnzm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gtlgpfhwrg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtqgdjfnkk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shzxlz.cn/gtdfiqbdvs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yuanzhike.top/gtyvvegzcj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ydjk.org.cn/gttznkpexm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtithxjyod.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gthrjgtnjz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtdbwtokaq.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gthzzgtruz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daria6918.cn/gtbcmmuoic.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtqciukqly.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.snrcjt.cn/gtiymvdoul.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtcjpuzdoi.html

[D15] 去重
来源：http://hz.zycfv.cn/gtbwhfjgog.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.birdmap.top/gtxrvcnuls.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtiowzoiqx.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtvzxwbeyw.html

TS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtfzpmfphp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258888.top/gtkffrzygr.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtxnqjakbb.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtcgfufnpy.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gttsgpjyon.html

[D16] 求和与平均值
来源：http://hz.hywenlv.cn/gtchhmyipq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gogol.net.cn/gtnxjffqhu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtrfqzzype.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gteyfvcxvb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtjcfsgxpf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.9152youxi.cn/gtivvlemeq.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gtawmqvwmk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtaneaayzz.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gtltmlgtus.html

[D17] 最大值与最小值
来源：http://hz.jqgfzy.top/gtkxvbaarv.html

Py:   max(arr);  min(arr)
来源：http://hz.smart0.xyz/gtbtmszwci.html

PHP:  max($arr);  min($arr);
来源：http://hz.birdmap.top/gtclyorhjw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xylfe.cn/gtzgjcfokr.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gtmuxlxtnc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtyjcktjoa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtyfqaapmn.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gtovkormlm.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gttkofuqsy.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtpthmcbdi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtvofohikq.html

PHP:  array_merge(...$nested);
来源：http://hz.tianlin.xyz/gtigisjkqr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gtsevhrywn.html

TS:   nested.flat();
来源：http://hz.xziqi.cn/gtvliyzqvj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nanxinkj.top/gtikpykfpi.html

Go:   // 手写双层循环
来源：http://hz.zhiwuduotai.top/gtynwzdkcn.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtpbwueese.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtunaqavdl.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gthqoziwmf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtoksecccx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtmeljwyvm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtztjmzwho.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtdwfcfwqz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.wangdashe.top/gtafyzkvbs.html

Go:   // 手写 map[string][]T
来源：http://hz.andypj.xyz/gtmjtcjodz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtbxdizped.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.0kj1m.cn/gtomygxfxl.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtyhqqnwhz.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtyxjmzelc.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtonrixjkd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtysmftiiw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenjidiqi.icu/gthxmgbbjn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.smart0.xyz/gtcxexkptj.html

Go:   // 手写 map[T]int
来源：http://hz.yueranfly.top/gtblkfrtjv.html

Ruby: arr.tally
来源：http://hz.daxiang520.top/gtvsjgqidu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.dashuyun.cn/gttymemoot.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtyftsllth.html

Py:   x in arr
来源：http://hz.shuidangran.top/gtkuaismym.html

PHP:  in_array($x, $arr, true);
来源：http://hz.bjfxy.top/gtlenlrvfh.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtcufnluyg.html

TS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtqbmglfbf.html

Java: list.contains(x)
来源：http://hz.0kj1m.cn/gtfrzuewpr.html

Go:   slices.Contains(arr, x)
来源：http://hz.svipenyu.cn/gtmdepvbsb.html

Ruby: arr.include?(x)
来源：http://hz.xuanzx.com/gtkjnfrjal.html

C#:   list.Contains(x)
来源：http://hz.ppjwa.cn/gtciiicxop.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtdrwgjyqd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pengpengdd.cyou/gtgxydcsxq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtlvqgztwc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtzbqxsium.html

TS:   [...arr];
来源：http://hz.xuanzx.com/gtfylcbhbi.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtedvvxvkr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.svipenyu.cn/gtpasgixsx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuetiantiany.cn/gtaghzegpk.html

C#:   new List<int>(list);
来源：http://hz.yonumen.top/gtiwuhftvv.html

[D23] reduce 累积计算
来源：http://hz.cucudq.cn/gtjpswmood.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.mhx1999.top/gtflqgessw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigufen.top/gtqekuajgo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtrhkqkitk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtgdpiskeg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.meibo888.top/gtrhxeqdkf.html

Go:   // 手写循环
来源：http://hz.pengpengdd.cyou/gtoudrjlci.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtlxduilch.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhijiandao.cn/gtfoiazxow.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtnszdbcxx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtaygziiio.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhixingplan.top/gtnqpuapgo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtywlznljm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtrvrvdheu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtfehtkzpu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gtkyigwhtq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtjrfoyjqm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtvvukfwtf.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gtmcrolcnu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtgqtxkswq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tianlin.xyz/gtlleghbyn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gtpkagheud.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhiwuduotai.top/gtrhifjbmu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuetiantiany.cn/gtakcssquo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtwiwnraui.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtnujezlmx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gttedhnseb.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtwykwlfbf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yonumen.top/gtwhupnmnj.html

PHP:  implode(", ", $arr);
来源：http://hz.ehwqpu.com/gtsoldifem.html

JS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtmjmgrgji.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtzihacvbd.html

Java: String.join(", ", list)
来源：http://hz.hongshengwenyu.top/gtmxhqxcih.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenzaomai.com/gtjtzmhqyj.html

Ruby: arr.join(", ")
来源：http://hz.snrcjt.cn/gtkvbiqkzz.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gtybanhktm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcsroiefh.html

E. 字符串处理
来源：http://hz.jqgufenzy.top/gtbtgwqexv.html

================================================================================
来源：http://hz.nanxinkj.top/gtvyvxgheh.html

[E01] 拼接字符串
来源：http://hz.xinyue.icu/gttbqahuiu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yonumen.top/gtubyhieae.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.smart0.xyz/gtbpdysrln.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinghuilouyu.cn/gtkhnocink.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtzwsbbbze.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guowangkeji.top/gtrdvgdtmy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtafukvpww.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtysivracb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtploejypw.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtmeuciety.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtsegnjbfq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtoirtkerk.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtjourdopq.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtmzkpwczd.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtryzqjapa.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtmofgpesk.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtaycpcozk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtdyxshudf.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gthgphfdfy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtjbijlezs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.smart0.xyz/gttddfuhwm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtbjskjxmc.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtnuiuiawb.html

Java: s.substring(1, 4)
来源：http://hz.cucudq.cn/gtkrdrhpqa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gtlfkchrgp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aizwys.cn/gtuervwgvb.html

C#:   s.Substring(1, 3)
来源：http://hz.hongshengwenyu.top/gtduoeyyas.html

[E04] 查找子串位置
来源：http://hz.nanxuanxn.top/gtjvzxuinu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtbxkoyjoe.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gtzznhpaci.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hysaishi.cn/gtbctzviii.html

TS:   s.indexOf("x")
来源：http://hz.jianghu66.top/gtjbagbvwx.html

Java: s.indexOf("x")
来源：http://hz.daria6918.cn/gtpaggroci.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigfzy.top/gtorjypfsp.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtnssjzvic.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gttjsjsfkt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.birdmap.top/gtctsoqpgm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guannengcc.top/gtbzekpkgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.feifeiyinyue.top/gtexhjygmq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ydzc1.top/gtncpekfrk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dianchejie.cn/gtokumrwkh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ehwqpu.com/gtpbclvxdj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtqflxyyim.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nwbrower.top/gtljiyimlx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnxiangtu.top/gtajafovcg.html

[E06] 替换子串
来源：http://hz.daria6918.cn/gtalgehbgi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtnfxrcbft.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shanyushiyangkeji.top/gtfphvpwkl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtxlsqknkp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtmuunkweq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtmhstgyhh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtckcpxbon.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgufenzy.top/gthsdoflfv.html

C#:   s.Replace("a", "b")
来源：http://hz.fzhhl.top/gttkglmjcu.html

[E07] 按分隔符拆分
来源：http://hz.ehwqpu.com/gteuispptt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.birdmap.top/gtpjndnkfl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtgdjviytg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.quarkkingdee.top/gtesqhkdey.html

TS:   s.split(",")
来源：http://hz.zhongyouzk.top/gtgelopdkc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtaphmvdok.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ppjwa.cn/gtviynjoop.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtonqeshit.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtnqutiuba.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtspoytavh.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtfjauqbql.html

PHP:  implode(",", $items);
来源：http://hz.zhaomingkeji.xyz/gtuaytammh.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtufkbuwni.html

TS:   items.join(",")
来源：http://hz.xziqi.cn/gtscfqqfkj.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtxaavnnoj.html

Go:   strings.Join(items, ",")
来源：http://hz.ydzc1.top/gtyvjtccfv.html

Ruby: items.join(",")
来源：http://hz.ppjwa.cn/gtczooivjc.html

C#:   string.Join(",", items)
来源：http://hz.jianghu66.top/gtslyspkqt.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtdzojyvun.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shuidangran.top/gtibsariwk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtqvlsylkg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gthorzqdud.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtzxhfwstc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gthiucvmbc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.tianlin.xyz/gtqsthsjph.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtxmmwpaml.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydzc1.top/gtehegludb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtqmwgynbr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ywan-chungtsiang.top/gthgrumwuh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtrtpngbjj.html

JS:   "7".padStart(3, "0")
来源：http://hz.aibaodan.cn/gttbepigjt.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtrsmahyvc.html

Java: String.format("%03d", 7)
来源：http://hz.9152youxi.cn/gtkhggxgzs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.c1oappe.top/gtklsnecbe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258888.top/gtmjqndcnj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.kuanghao11.cn/gthbitdsxx.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtodbpbskv.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gteluffoct.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gtxsibaorl.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtxjklvsui.html

TS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtbekqjoih.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenzaomai.com/gtpcbdyuht.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xinyue.icu/gtvrsdsdsc.html

Ruby: s.reverse
来源：http://hz.dianchejie.cn/gtjjxogmfc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtyyhjluio.html

[E12] 统计某字符出现次数
来源：http://hz.shangyingyoupin.top/gtjztslcty.html

Py:   s.count("a")
来源：http://hz.yuanzhike.top/gtrkrmwcsc.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtdsihnywu.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtdwdkcvaw.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtovyadbof.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtoltbjxeu.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtmipofvpg.html

Ruby: s.count("a")
来源：http://hz.hnqzz.top/gtpdtjeasg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtkfzjxfoz.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gtpxuntjuq.html

Py:   for ch in s: print(ch)
来源：http://hz.hnxiangtu.top/gtpmxrsire.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtbszbrkzk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtfpinrrtx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtetwzawdc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tanke756.top/gtnxbobbis.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtdlytpxjs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yanxiufei.cn/gtqjdpqwqj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangkeji.top/gtcijtnhvi.html

[E14] URL 编码与 Base64
来源：http://hz.0kj1m.cn/gtuaauatdb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tanke756.top/gtxodakery.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shuidangran.top/gtrbwbmlmz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guannengcc.top/gtmqltzjqq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhoulong.xyz/gtbgvjrdwu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtwefcmliw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtqthjeklb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtaukynjqq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgfzy.top/gtebglzwko.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtebfhpfzp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtfqrwutst.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtfuwcrhbd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gtdtnrbatg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinghuilouyu.cn/gtqxxiddsy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhijiandao.cn/gtfocvybae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtquobehcf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jiagoushi.top/gtoyzojqgl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhiwuduotai.top/gtdzgjopds.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtaiutwbmc.html

Py:   f"{1234567:,}"
来源：http://hz.feifeiyinyue.top/gtqlalbsha.html

PHP:  number_format(1234567);
来源：http://hz.cashguo.top/gtulwmlhuj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtkvbnqrqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.vqdsnc.cn/gtiazroxes.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gtbhzpjuzf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sufxvd.cn/gtqouipugn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtwmpwdjac.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtsontgckc.html

[E17] 首字母大写
来源：http://hz.hnxiangtu.top/gtolyiccqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtkjksripx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtnxqahmov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangtech.top/gtuorqnkkp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuxming.cn/gtzwiigzcp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtynqqhqsp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gthmnnqmgr.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtqgplmjdr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtnkguowqb.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gttxwfaygh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtmuqyaboy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gtzhvvlxnx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtytafjryb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtuvmmpxia.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtnggglzqd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtqoroakix.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtbawkefuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258888.top/gtekyvsxit.html

[E19] 多行文本按行拆分
来源：http://hz.sysykeji.top/gtendfrvwp.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtlbshgqzd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aizwys.cn/gthuagrejt.html

JS:   s.split(/\r?\n/)
来源：http://hz.gzhubu.top/gtnwkkzhbt.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtrhtbsqcv.html

Java: s.lines().toList()
来源：http://hz.ywan-chungtsiang.top/gtpghmkugz.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtffgpfqas.html


<!-- 参考信息 -->