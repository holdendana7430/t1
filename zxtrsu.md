代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.9152youxi.cn/gteptrpbhn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtakkwmckx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtawfvsxbo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtdogjtbim.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gtjpmnfqwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtpcihnoru.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shuidangran.top/gtdbfddnph.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guowangkeji.top/gteupkcwnd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.mhx1999.top/gtcduzemez.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pengpengdd.cyou/gtidmbxrhx.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtjpwtetlo.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gtlruivhvg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xingfuxueyuan.xyz/gtejgkbmnc.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtoaasmqsf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangshuangyany.cn/gtwhyaxutb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtmdkwouta.html

[D15] 去重
来源：http://hz.bjfxy.top/gtqjaithii.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.bjfxy.top/gttbqxvabv.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtuniqhitj.html

JS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtvrvbksxr.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtkfvdzpah.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtdlvfqpxb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.quarkkingdee.top/gtwnafmyal.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtotdftqbo.html

C#:   list.Distinct().ToList()
来源：http://hz.cashguo.top/gtpfwpaxak.html

[D16] 求和与平均值
来源：http://hz.jiagoushi.top/gtphgfplyy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtaowimlli.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtzenhdrbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtubocqmtp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtlwqsiqup.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gttmoqnugw.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtaaqjqwow.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shanyushiyangtech.top/gtvjgflgss.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gtckqazdrd.html

[D17] 最大值与最小值
来源：http://hz.yangfankeji.com/gtnetkubqj.html

Py:   max(arr);  min(arr)
来源：http://hz.fengsongda.top/gtumjnqahh.html

PHP:  max($arr);  min($arr);
来源：http://hz.dashuyun.cn/gtqmrjakjo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtddszjkzc.html

TS:   Math.max(...arr);
来源：http://hz.9152youxi.cn/gtbktjyhvm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtezzxarum.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.c1oappe.top/gtaycykpdx.html

Ruby: arr.max;  arr.min
来源：http://hz.yueranfly.top/gtbudjatxj.html

C#:   list.Max();  list.Min()
来源：http://hz.c1oappe.top/gtqaycycbp.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtzbkovgcu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gthlvbhuqo.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gteiszrcdc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tanke756.top/gttkikbjlt.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtbofnjsid.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhiwuduotai.top/gtcxhlygpw.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtttzhbeqv.html

Ruby: nested.flatten
来源：http://hz.ppjwa.cn/gtqqdkueuv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tianlin.xyz/gtzxajfejn.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtribrltkh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gotoacloud.top/gtrlfghfjq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhijiandao.cn/gtenjpbdpg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtuoksdykq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtwuwsqhxk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cucudq.cn/gtvqnxqdwg.html

Go:   // 手写 map[string][]T
来源：http://hz.c1oappe.top/gtghhlbudh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gtrdlfwpbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nwbrower.top/gtmgzusjrj.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtlisijbfj.html

Py:   Counter(arr)
来源：http://hz.jyoumei.cn/gtvvpbprxz.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gthadtcyem.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yanxiufei.cn/gtxszxnquw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtqordtyyf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtqobsujhg.html

Go:   // 手写 map[T]int
来源：http://hz.shanyushiyangtech.top/gtaqxfyane.html

Ruby: arr.tally
来源：http://hz.sweek.top/gtvzajnxnh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtpethfzlg.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtxymvrhiy.html

Py:   x in arr
来源：http://hz.aibaodan.cn/gtxydqifzy.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtjxuasxsh.html

JS:   arr.includes(x)
来源：http://hz.xinyue.icu/gtrbfsplwr.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtivlcqwbu.html

Java: list.contains(x)
来源：http://hz.yuxming.cn/gtojcpuwhi.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinghuilouyu.cn/gtwydysypm.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtvnqxxdaa.html

C#:   list.Contains(x)
来源：http://hz.kuanghao11.cn/gtcujcxnrm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gthqfzoets.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgufenzy.top/gtssdruipw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sufxvd.cn/gtdfvsawls.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xuanzx.com/gtzczsmwpg.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtpdkhkloe.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtxgqaijkc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yueranfly.top/gtohpjlolx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtpsgtqzyg.html

C#:   new List<int>(list);
来源：http://hz.haohaochexian.top/gtebtcirgm.html

[D23] reduce 累积计算
来源：http://hz.fengsongda.top/gtnpngpims.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtpycepusf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtbjkjbrxn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuetiantiany.cn/gtuaborbwy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuanzhike.top/gtbqnevqfz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guannengcc.top/gtrbzzctef.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtwlkycpew.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gtibejjltw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hongshengwenyu.top/gtxmyjsyig.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gthgzwqmes.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtcfxdetce.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtowshdhfd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fzhhl.top/gthrgjrowv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydzc1.top/gtstiozequ.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xinyue.icu/gtbcrfntgw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangshuangyany.cn/gtqwyueaof.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zdqjudy.top/gtzhaitoay.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gtrpcwxths.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtaofswkzr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shuidangran.top/gtdoyrpvww.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangkeji.top/gtnixiigkt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtvywkppwb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gtgpidohfu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtncteokrm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gthuncoehf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtnolhckht.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtzfioyocp.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtiinzoeud.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxuanxn.top/gtxtgyztgn.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtujulzohl.html

JS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtpuhyvnwa.html

TS:   arr.join(", ")
来源：http://hz.xuetiantiany.cn/gtaolrfimn.html

Java: String.join(", ", list)
来源：http://hz.shuidangran.top/gtqlgpotrj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtzpfacwpi.html

Ruby: arr.join(", ")
来源：http://hz.smart0.xyz/gtjhgbsbky.html

C#:   string.Join(", ", list)
来源：http://hz.guannengcc.top/gthyydywfg.html

================================================================================
来源：http://hz.yvedp.cn/gtynpbkbfm.html

E. 字符串处理
来源：http://hz.cheryme.top/gtorpvrwhq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlfzidfbq.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtmwenrnxb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gzhubu.top/gtcltdtgsj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtzfeycchg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtbwbnhhpl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtctxfzqot.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sufxvd.cn/gtepiqfwie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yueranfly.top/gtmplyuuov.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigufen.top/gtwlwlgxcf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gaohongyu789.top/gtabapjujh.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gthhtjjxks.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtkhikpjhh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtzunniiqa.html

JS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtiosnsqsz.html

TS:   "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtoecyakmq.html

Java: "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtqothkynu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jqgfzy.top/gtxxafdjlp.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtgojofpcf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ivvv.top/gtqasdayxo.html

[E03] 截取子串
来源：http://hz.nanxinkj.top/gtebsymlkt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtxdjhvxrt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtgaconows.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtnpfnafry.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtiyvefjng.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtkjggrqnt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtktnqgghd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.c1oappe.top/gtgeittojd.html

C#:   s.Substring(1, 3)
来源：http://hz.yvedp.cn/gtctegwhmp.html

[E04] 查找子串位置
来源：http://hz.jlsjyb.cn/gtdhiuhzri.html

Py:   s.find("x");  s.index("x")
来源：http://hz.iojbl.cn/gtdslxktdm.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangtech.top/gtmctaojov.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinqigufen.top/gtbvnpstej.html

TS:   s.indexOf("x")
来源：http://hz.daxiang520.top/gtchgzrxzx.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtntmsxbtq.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtfkwrsvku.html

Ruby: s.index("x")
来源：http://hz.ydzc1.top/gtdsvqsjid.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtpbzmoeen.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gtrerfrjsy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nwbrower.top/gtnbcmmacm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtzxzvpahx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtnttyjswj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.vqdsnc.cn/gtwngnzbbz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgfzy.top/gteavvvswk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shzxlz.cn/gtrejqzjwf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangkeji.top/gtbpcdpmak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ehwqpu.com/gtfgwpkrmf.html

[E06] 替换子串
来源：http://hz.yangfankeji.com/gtamfiiqkj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtukguqcqs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.guannengcc.top/gtzuwitdub.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtjkltinkz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtxomvoiyb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtetsubrbx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dianchejie.cn/gtcwnaynyp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtqsxxtgbr.html

C#:   s.Replace("a", "b")
来源：http://hz.daxiang520.top/gtbadapfdt.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtzdwyycva.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxinkj.top/gtxgsuicxs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pycfn.com/gtorthuhum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangshuangyany.cn/gteyxklefm.html

TS:   s.split(",")
来源：http://hz.zhengqikj.top/gtahtlpdjt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtoijxsqgw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gtaoirwkxl.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtzytykypk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wangshuangyany.cn/gtcslefsnq.html

[E08] 数组按分隔符合并
来源：http://hz.xuanzx.com/gtjbymijsj.html

Py:   ",".join(items)
来源：http://hz.jqgufenzy.top/gtgffyweom.html

PHP:  implode(",", $items);
来源：http://hz.jyoumei.cn/gteqkkcczm.html

JS:   items.join(",")
来源：http://hz.yj20258.top/gtxpeqachv.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gteuiqskzr.html

Java: String.join(",", items)
来源：http://hz.vqdsnc.cn/gtqumnojio.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtnknenfrr.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtwygpefmn.html

C#:   string.Join(",", items)
来源：http://hz.quarkkingdee.top/gtopypwvau.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtuzdaqlad.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.9152youxi.cn/gtgqoolipp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.haohaochexian.top/gtvfwfuvjo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtgfopjfmj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtzfnxtosq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ydjk.org.cn/gtuqftygrg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtrbuubdre.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxuanxn.top/gtfkcbvnts.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.haohaochexian.top/gtvfrtlwlg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ppjwa.cn/gtkerqpudw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtrccmaown.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtozcygznp.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gticnkgbnn.html

TS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtkcponbar.html

Java: String.format("%03d", 7)
来源：http://hz.jqgfzy.top/gtfxzxvuio.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gtzeuqhkpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jiagoushi.top/gtgdkaxhzj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtzhcmfhnu.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtrnadlpro.html

Py:   s[::-1]
来源：http://hz.jyoumei.cn/gtirmrxgif.html

PHP:  strrev($s);
来源：http://hz.jqgufenzy.top/gtumamjbya.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtsznixeef.html

TS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtgvkjhftz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtrdgmcugu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtticovwqa.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtsdnwbwuy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhengqikj.top/gtuxyfmnyg.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtjlnclgrl.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtuhronlpz.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtjnlhfcdq.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtudgiqkil.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtnkwwowzm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtellmgwyq.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtxcaogpsh.html

Ruby: s.count("a")
来源：http://hz.xuetiantiany.cn/gtfshldxqd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.svipenyu.cn/gtxnshilwf.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtxewbbfhh.html

Py:   for ch in s: print(ch)
来源：http://hz.yuanzhike.top/gtvwmkxavq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.bjfxy.top/gtmcafneuu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtnqbiymzn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtvghxvmyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yueranfly.top/gtcfqbgklv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtlsmesqki.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtnemocprk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtigihkxie.html

[E14] URL 编码与 Base64
来源：http://hz.vqdsnc.cn/gttyhlyxcs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtjfypvbaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.0kj1m.cn/gteecwoxjs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangtech.top/gtdjumfnah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtuvigytin.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtlejwbidw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtnlvpciwr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtnivodmbn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aibaodan.cn/gtektxaybh.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtqcodgnaw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj202588.top/gtnaomxuok.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgufenzy.top/gtnemrhpcr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yangfankeji.com/gtlxtizgfh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.birdmap.top/gtovystain.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtuabclkpv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cashguo.top/gtihvhfrph.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtnvipxauu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.wangdashe.top/gthglaupep.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gtouicjcxs.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtfpsmfbcn.html

PHP:  number_format(1234567);
来源：http://hz.fengsongda.top/gtsjoyhbgz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtvcvdhouk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xinyue.icu/gtgdxuyujh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.0kj1m.cn/gthndcxmqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nanxuanxn.top/gtgkbojuib.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gteojanvwd.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtnuodqfjo.html

[E17] 首字母大写
来源：http://hz.52xcode.cn/gtgrukmaic.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtnlakcyjl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtpjhznjws.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtudehztvl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gtgquqikvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yueranfly.top/gtkuyomssg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtuzcdpzpe.html

Ruby: s.capitalize
来源：http://hz.hongshengwenyu.top/gtphysziio.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtfxnoznop.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtqzqwdrli.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtkbicbmoi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hammf.cn/gtfsmaxgyx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtazczijgp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtabhbseik.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gtbfynqbbl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gtrlttduxd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtzdegbmay.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258888.top/gtollzdayz.html

[E19] 多行文本按行拆分
来源：http://hz.xuetiantiany.cn/gtjbqsmvng.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtpbmioxne.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gtoamdpfqk.html

JS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtcmhbiuzc.html

TS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gthlsxanmj.html

Java: s.lines().toList()
来源：http://hz.chenjidiqi.icu/gtbrdyhzpx.html

Go:   strings.Split(s, "\n")
来源：http://hz.yongpay.top/gtyqdlowzt.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtbtebituk.html

C#:   s.Split('\n')
来源：http://hz.nanxinkj.top/gtbfocglpi.html

[E20] 判断字符串是否为空
来源：http://hz.shanyushiyangkeji.top/gtshwrurbo.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtunwipgul.html


<!-- 参考信息 -->