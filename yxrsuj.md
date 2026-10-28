代发 wailian999

[D15] 去重
来源：http://hz.ehwqpu.com/gtzrimyemv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gthuohyccs.html

PHP:  array_unique($arr);
来源：http://hz.yuxming.cn/gtuqnodxir.html

JS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gthphvoamm.html

TS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtabnrcmij.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gtexbglhav.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxinkj.top/gticqctojv.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtfmqyukwj.html

C#:   list.Distinct().ToList()
来源：http://hz.svipenyu.cn/gtwmpsrhwn.html

[D16] 求和与平均值
来源：http://hz.ehwqpu.com/gtvtpzyvff.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangtech.top/gtppxyuvig.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.316326.xyz/gttcufoias.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtrrucllgw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtsdtqrqwy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtebtskojg.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtizghkggk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtllkgyyal.html

C#:   list.Sum();  list.Average()
来源：http://hz.daxiang520.top/gtbggxsiku.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtubiiuedm.html

Py:   max(arr);  min(arr)
来源：http://hz.wangshuangyany.cn/gtjqaohcqk.html

PHP:  max($arr);  min($arr);
来源：http://hz.feifeiyinyue.top/gtfkacqiju.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtjuzketwx.html

TS:   Math.max(...arr);
来源：http://hz.ybcxt.top/gtebytdqwl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenzaomai.com/gtejypymbv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.svipenyu.cn/gtonmdvmyx.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258.top/gtqibpcbau.html

C#:   list.Max();  list.Min()
来源：http://hz.bjfxy.top/gtvwuwymal.html

[D18] 扁平化嵌套数组
来源：http://hz.ydzc1.top/gtgcemnwdh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gtxrnujcxd.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtvvfiwnrn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gotoacloud.top/gtpuvtslqj.html

TS:   nested.flat();
来源：http://hz.zhixingplan.top/gtrextymsv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.andypj.xyz/gtdhzqwrwm.html

Go:   // 手写双层循环
来源：http://hz.nanxinkj.top/gteryxswhk.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtwtcfammk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.9152youxi.cn/gtpghimblg.html

[D19] 按字段分组
来源：http://hz.iojbl.cn/gtmdhojofj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtfxtobejf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xziqi.cn/gtgcciaaxc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtpusbzonv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenjidiqi.icu/gtdlzuklip.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jqgfzy.top/gtqopqjsau.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtvyzvxpvn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zycfv.cn/gtlssczsqr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtlylavqlp.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtuxawhcni.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gtjnhccnoz.html

PHP:  array_count_values($arr);
来源：http://hz.tianlin.xyz/gtxbglheap.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtooqhvwnn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtomrzizxe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.aizwys.cn/gtjaowavsu.html

Go:   // 手写 map[T]int
来源：http://hz.zhoulong.xyz/gtojupanzu.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtxchaillh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.birdmap.top/gtzkoawlmv.html

[D21] 判断是否包含某元素
来源：http://hz.zhiwuduotai.top/gteakoqaeh.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtpudifnha.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cheryme.top/gtqpmcklbo.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtwfhmaflf.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtkoewvbzr.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtapvzbgjd.html

Go:   slices.Contains(arr, x)
来源：http://hz.svipenyu.cn/gtpkgyreje.html

Ruby: arr.include?(x)
来源：http://hz.snrcjt.cn/gtynbtrtvs.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtxgvzzjgf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtebwnzyod.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtfglmowse.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtmixuimhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhaomingkeji.xyz/gteeshneup.html

TS:   [...arr];
来源：http://hz.xylfe.cn/gttkxbbaeb.html

Java: new ArrayList<>(list);
来源：http://hz.jinyuanbaomall.cn/gtghedotzp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ybcxt.top/gtzhndsvki.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yonumen.top/gtuqdjsedx.html

C#:   new List<int>(list);
来源：http://hz.dianchejie.cn/gtlzzypxuj.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtorwispij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gthkttdkuk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtjolmyxzn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtazgiogjv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gttbjlvkhr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtjvbryenc.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtwbgvvutt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tian-w.cn/gtowhtxiis.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhaomingkeji.xyz/gtdfletjzy.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gttdcotizd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guannengcc.top/gtqjbanfsh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gotoacloud.top/gtzuzhlkgr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtkxafzwxp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtiebxynep.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yongpay.top/gthvbriqxh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gtzwpvzgpe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hywenlv.cn/gtmtedtlix.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ppjwa.cn/gtvecrmysm.html

[D25] Set 集合去重与交并差
来源：http://hz.xylfe.cn/gtilmpytfv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtjeyvzyfz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yueranfly.top/gtwoevxgjy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.316326.xyz/gtznackokl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gtkogvsmqy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shangyingyoupin.top/gtqusbxalx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtnbmygoxw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.iojbl.cn/gtultwkfza.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtddtmohxu.html

[D26] 数组转字符串
来源：http://hz.ydzc1.top/gtqqctgrel.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gteswsunpu.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gtlzuhovhs.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtlhmlefrc.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtyysvrtbw.html

Java: String.join(", ", list)
来源：http://hz.ydzc1.top/gtkgxjjplc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gtfgtpxqde.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtemgsdait.html

C#:   string.Join(", ", list)
来源：http://hz.birdmap.top/gtslcsvdug.html

================================================================================
来源：http://hz.meibo888.top/gtxonwhkun.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtgbudpmte.html

================================================================================
来源：http://hz.hnqzz.top/gtwtmpfwte.html

[E01] 拼接字符串
来源：http://hz.ybcxt.top/gtenhuxiog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.vqdsnc.cn/gttdokhjix.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinyuanbaomall.cn/gtofpruvnx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtprzilzde.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtxwenoxcg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gtzolhdqvd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gaohongyu789.top/gteteynlla.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ehwqpu.com/gtqhagmeti.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.mhx1999.top/gtzqdztsgp.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtasypzuge.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtbanmtezn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xuanzx.com/gthaxkrbrt.html

JS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtumlcrkje.html

TS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtkntchzff.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtoptvptec.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pengpengdd.cyou/gtludmefyn.html

Ruby: "ab" * 3
来源：http://hz.tanke756.top/gtfrivfqxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gtqyzqcoes.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtmizimdek.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinghuilouyu.cn/gtwxvnvsii.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xylfe.cn/gttgkgsqqb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtgwmatbhn.html

TS:   s.slice(1, 4)
来源：http://hz.tian-w.cn/gtizjxsxlq.html

Java: s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtzjivqqry.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtdchznypx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.mhx1999.top/gtfuiremrr.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gtmcbijzyx.html

[E04] 查找子串位置
来源：http://hz.mhx1999.top/gtwownjshz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj202588.top/gtiygjccoj.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gtxmuvidrb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtnvuomieb.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gthdpqzrbl.html

Java: s.indexOf("x")
来源：http://hz.ybcxt.top/gtulpnuuuy.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtajirbqgg.html

Ruby: s.index("x")
来源：http://hz.hnqzz.top/gthsqisfwi.html

C#:   s.IndexOf("x")
来源：http://hz.nanxinkj.top/gtbfsnosyd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtubognaqc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xylfe.cn/gtjvwijqjp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yongpay.top/gtftxybdhv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gticgyzwwv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinghuilouyu.cn/gtihrqakrl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtatqcgthz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtwxoqkkeo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydjk.org.cn/gtakarolew.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhongyouzk.top/gtyuwgsbpn.html

[E06] 替换子串
来源：http://hz.shanyushiyangkeji.top/gtqtwtfwnc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gtzhytvazz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtzzpvwzrg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtintclbrb.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtawqyzxpg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gttzvkuqlu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.mhx1999.top/gtdpyejnxf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtjmnmvgoo.html

C#:   s.Replace("a", "b")
来源：http://hz.yvedp.cn/gtnsipbgtm.html

[E07] 按分隔符拆分
来源：http://hz.bjfxy.top/gtkmsmzwjd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gtkdmwlanz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daria6918.cn/gtmygnauvt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.haohaochexian.top/gtykgefwir.html

TS:   s.split(",")
来源：http://hz.cqqwz.cn/gteduydfmk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.9152youxi.cn/gtralbmgcl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtsnvdlfuo.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtfmutqzfh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydzc1.top/gtdnhcjtaz.html

[E08] 数组按分隔符合并
来源：http://hz.jlsjyb.cn/gtkktpygfm.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gttgdrngki.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtaokydomj.html

JS:   items.join(",")
来源：http://hz.yj202588.top/gtqlavnnyx.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtsjgaispu.html

Java: String.join(",", items)
来源：http://hz.yueranfly.top/gtmrbdhyli.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtyfevlffh.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtmxjhyjce.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtjvjcwqsf.html

[E09] 去除所有空白字符
来源：http://hz.zhijiandao.cn/gtbkixxkrp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtolhpemkg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhiwuduotai.top/gtgrhkctur.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtvhgcymno.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtxhmtqfxf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jiagoushi.top/gtzcinpite.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.svipenyu.cn/gtkljbihav.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sysykeji.top/gtoatuflnk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pengpengdd.cyou/gtiozrbxtt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtnutehydt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ybcxt.top/gtqzlxrvhf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.mhx1999.top/gtvwrbuuhc.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigfzy.top/gtdsoudimo.html

TS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtbtukkdfi.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gtuxnuxaow.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.mhx1999.top/gtribqtlcg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtkoigncxn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.andypj.xyz/gtxlqbygtw.html

[E11] 反转字符串
来源：http://hz.hnqzz.top/gtwbrifvpc.html

Py:   s[::-1]
来源：http://hz.chenlongwang.top/gtbiqfvpuv.html

PHP:  strrev($s);
来源：http://hz.haohaochexian.top/gtdkcwsmgy.html

JS:   [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtxfhcaauy.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtqioqqrsu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.9152youxi.cn/gtwqapycbv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtdtgjonbi.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtcjdcrzsi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtheztowln.html

[E12] 统计某字符出现次数
来源：http://hz.ivvv.top/gtxwnwziqg.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtwxfbhzuu.html

PHP:  substr_count($s, "a");
来源：http://hz.zycfv.cn/gtevvdsbex.html

JS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtodweavif.html

TS:   s.split("a").length - 1
来源：http://hz.sysykeji.top/gtrbuvdssn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pycfn.com/gtuoyphuvw.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtnothtkvg.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtixsxtvgn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtunuymgfm.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtvdpnwgfo.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtfaczidyo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhijiandao.cn/gtluhhxqjd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtkgducnvr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtbfjyjkmr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nwbrower.top/gtwzsgggnu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gaohongyu789.top/gtthmbpivh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.tianlin.xyz/gtdriyxiqm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtklciokto.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtlkdxurnv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cheryme.top/gtiaoxtgdf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cucudq.cn/gtahamblbr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gttywurkja.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj20258888.top/gtblccpbql.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ywan-chungtsiang.top/gtslsiqcnb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gtcncoxjyj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ivvv.top/gtfvcetkoj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tian-w.cn/gtohxwekwo.html

[E15] HTML 转义 / 反转义
来源：http://hz.daria6918.cn/gtopfludpj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258.top/gtdakpuvbn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtafsmwhno.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtupasnrnl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daria6918.cn/gtjpgmfguf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhiwuduotai.top/gtrfdzihdy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenjidiqi.icu/gtfgbreacq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtpzgragov.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtxhbhjjwa.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gticrkujey.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gtmdarrcix.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtteqwmpnu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gthaifloyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhiwuduotai.top/gtzpphvmcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhengqikj.top/gtinbxyukt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtvcyhqgnd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtgeraetap.html

C#:   1234567.ToString("N0")
来源：http://hz.xuetiantiany.cn/gtraxivcsb.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtukrxixji.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtuqlrajyn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pycfn.com/gtektuqpfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtzwclqnos.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtutuebtvk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnqzz.top/gtzsxztkuw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuanzx.com/gtnkevounq.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtxpqipsda.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtbybkuvtg.html

[E18] 模板占位符替换
来源：http://hz.bjfxy.top/gttbujlzfo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtzjhpracm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zycfv.cn/gtcwtbdryq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtwhgowqkc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guowangkeji.top/gtzwptvdfv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gtnexqzvde.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtzwbpvbyc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.316326.xyz/gtlcjpealv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.iojbl.cn/gtowcgpsel.html

[E19] 多行文本按行拆分
来源：http://hz.c1oappe.top/gtjhhaufse.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtaccfynzx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ydjk.org.cn/gtwhmslqis.html

JS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtkghblxjl.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtuynerzzc.html

Java: s.lines().toList()
来源：http://hz.sxryk.cn/gtlrcgzgms.html

Go:   strings.Split(s, "\n")
来源：http://hz.yanxiufei.cn/gtvasibnjk.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtdrerlazf.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtbmryibuw.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gtmzbnhgsl.html

Py:   if not s:
来源：http://hz.nanxuanxn.top/gtftazkkun.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtacolyakr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuxming.cn/gteexdbbnj.html

TS:   if (s === "") {}
来源：http://hz.xuanzx.com/gtzzawvbkg.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtxauufqoa.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtaolehfxe.html

Ruby: if s.empty?
来源：http://hz.zhoulong.xyz/gtpmpjbycs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtseicowfl.html

[E21] 超长截断加省略号
来源：http://hz.fengsongda.top/gtkkbdsbeh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gogol.net.cn/gtiqhioars.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxuanxn.top/gtpklibtbw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.haohaochexian.top/gthumrextn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtjqjylczr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtdteztdal.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtsiykqeex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gttighcmby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jqgfzy.top/gtenwhrocf.html


<!-- 参考信息 -->