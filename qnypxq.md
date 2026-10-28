代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtudeamydq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cucudq.cn/gtaoslpznd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gotoacloud.top/gtchzayqvc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinyuanbaomall.cn/gtuamtuikb.html

[D11] 反转数组
来源：http://hz.chenzaomai.com/gtchrxricy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hongshengwenyu.top/gtvfmugxns.html

PHP:  array_reverse($arr);
来源：http://hz.nanxinkj.top/gtlfoqlnlo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtcnernizh.html

TS:   [...arr].reverse();
来源：http://hz.gogol.net.cn/gtvbukrafd.html

Java: Collections.reverse(list);
来源：http://hz.cheryme.top/gtdmzpkucw.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtxwcykndx.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtmtoqsnmb.html

C#:   list.Reverse();
来源：http://hz.jinqigfzy.top/gtqjzxcedk.html

[D12] 查找元素下标
来源：http://hz.guannengcc.top/gtaqfwhgwk.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtfotskxtv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cqqwz.cn/gtkkiiwjkv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gthvmenagw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtuirkuoyv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtvciimusc.html

Go:   slices.Index(arr, x)
来源：http://hz.yangfankeji.com/gtikcnvypg.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtoiyqsyxy.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtmpadekcj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gthwycvlav.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ehwqpu.com/gttqrirzas.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtriahigdt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gtsatkaurj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtiqdpvgzd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gotoacloud.top/gthwuvvgnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.fzhhl.top/gtjjhlnmum.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtwnynfujt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gtjjemalzo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtalijxlmn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtsydhwvdh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtiioezgyw.html

JS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtbsrieivm.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtihvihsbr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hnqzz.top/gtdjuaabga.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtiypgdydb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.pengpengdd.cyou/gtflugkabu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuxming.cn/gtogqmgogj.html

[D15] 去重
来源：http://hz.svipenyu.cn/gtwundnzlg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtakcwocdc.html

PHP:  array_unique($arr);
来源：http://hz.wangdashe.top/gtctdcdack.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtmxeyqrlk.html

TS:   [...new Set(arr)]
来源：http://hz.hysaishi.cn/gtngzbqwaa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuanzhike.top/gtnskouzja.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258.top/gtoguwisbs.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtfymduqli.html

C#:   list.Distinct().ToList()
来源：http://hz.smart0.xyz/gtagwvagsb.html

[D16] 求和与平均值
来源：http://hz.snrcjt.cn/gtfsnlztzb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gtmirhsbuy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.9152youxi.cn/gtlsqoqdtx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtgeipjrod.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gtacwuxqof.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xziqi.cn/gtpserheqt.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtzglztckz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinyuanbaomall.cn/gtumafkuov.html

C#:   list.Sum();  list.Average()
来源：http://hz.quarkkingdee.top/gtdpzowuth.html

[D17] 最大值与最小值
来源：http://hz.andypj.xyz/gtucwngxkf.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtvlugrzkx.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gttevatklm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtmvcspdjx.html

TS:   Math.max(...arr);
来源：http://hz.ppjwa.cn/gtcnwxqlpu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhixingplan.top/gtlmbbgoov.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.mhx1999.top/gthaogcreq.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtbrpqfflh.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtjeqrzeqc.html

[D18] 扁平化嵌套数组
来源：http://hz.sysykeji.top/gtaellzvov.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.fengsongda.top/gtnmznvjac.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gthaejmuau.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtkxunlnrw.html

TS:   nested.flat();
来源：http://hz.yj20258888.top/gtyjwkvyoo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gteizwzkgk.html

Go:   // 手写双层循环
来源：http://hz.guowangkeji.top/gtkwcixmiw.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtggjxhyhn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yvedp.cn/gtmmegnxwm.html

[D19] 按字段分组
来源：http://hz.andypj.xyz/gtkyrxuhjj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtnauaetkr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtowulmfhc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gthifhezsw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtjukzrfbo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydzc1.top/gtlvaimvuy.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtktldyqck.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtkawhlcyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258888.top/gtlzycmukl.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtuccmvxgk.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtiqwsgwko.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gtyqodkkuy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtjbcibskr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtlrcguqbz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ybcxt.top/gtkigvfbsn.html

Go:   // 手写 map[T]int
来源：http://hz.daria6918.cn/gtpjzrhqle.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtslzrktyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shangyingyoupin.top/gtxvurcsoq.html

[D21] 判断是否包含某元素
来源：http://hz.sysykeji.top/gtlercmoca.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtwhfbrizx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtwyeavhzm.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtiasyqvsl.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtxxygrklj.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gtleuwkmka.html

Go:   slices.Contains(arr, x)
来源：http://hz.xinyue.icu/gtdfwwkbru.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtaxixfcoo.html

C#:   list.Contains(x)
来源：http://hz.52xcode.cn/gtowozoxix.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gtpmmecvvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gterrgfskr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gtdwbgjdvc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gtzcywvdvd.html

TS:   [...arr];
来源：http://hz.316326.xyz/gtlgetifjj.html

Java: new ArrayList<>(list);
来源：http://hz.guannengcc.top/gthszcxvop.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gthkcispdk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.pengpengdd.cyou/gtqoakkcmg.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtfeqntgtv.html

[D23] reduce 累积计算
来源：http://hz.feifeiyinyue.top/gtuqtvrooe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtxbvfjgcg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.bjfxy.top/gtnuphlbwl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hongshengwenyu.top/gtubbagwbl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtjpeaatml.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenzaomai.com/gtdprzynyt.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtpchigkct.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ydjk.org.cn/gtpoeuklul.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gtgqwrfyfy.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gtozpuljon.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhixingplan.top/gtacocpvnw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zdqjudy.top/gtfvgqesfg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hfpthk.cn/gtyurmfkru.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtdofztrom.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xziqi.cn/gtzyplcgrk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fzhhl.top/gtolwdsyaw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtwrxlqyuf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtlfwqdfcc.html

[D25] Set 集合去重与交并差
来源：http://hz.daxiang520.top/gtnuadnoym.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtrgxittpq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinyuanbaomall.cn/gtgpruemke.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fengsongda.top/gtbcoymdhn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gaohongyu789.top/gtyjzszvzi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gttftvniwk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yangfankeji.com/gtslzgrqwj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.vqdsnc.cn/gtsicgquhf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ehwqpu.com/gthcwmtasv.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtnbpuscko.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cucudq.cn/gteweagjol.html

PHP:  implode(", ", $arr);
来源：http://hz.zhijiandao.cn/gtkpvugwvw.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtkcvmnejb.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtqiwsktgm.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtfbqfuhcs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.52xcode.cn/gtculbreyg.html

Ruby: arr.join(", ")
来源：http://hz.aibaodan.cn/gtkbgogmxm.html

C#:   string.Join(", ", list)
来源：http://hz.cashguo.top/gtkqxlglys.html

================================================================================
来源：http://hz.ppjwa.cn/gtgfvzbwnz.html

E. 字符串处理
来源：http://hz.gotoacloud.top/gtbtdwzprk.html

================================================================================
来源：http://hz.nwbrower.top/gtsmeiopje.html

[E01] 拼接字符串
来源：http://hz.cdnleiting.top/gtodvqsevu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gthmeftgfx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ivvv.top/gtkxorviid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtgjguvqcs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtupshyhzu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxinkj.top/gtyhjfpkln.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sysykeji.top/gtssxhphlb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtiazuxhdi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj202588.top/gtwdzkhenu.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtlyspihxl.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtnldyctwh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtrjkltyud.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtxwdxukwb.html

TS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gtqydpqgar.html

Java: "ab".repeat(3)
来源：http://hz.ivvv.top/gtvxvtvjyh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhixingplan.top/gtyfwsztcd.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtzngsfydo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258.top/gtbmiwidmc.html

[E03] 截取子串
来源：http://hz.shangyingyoupin.top/gtklzqztvd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cdnleiting.top/gtbtxkyeyt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuetiantiany.cn/gtjodeqqga.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pengpengdd.cyou/gtaojklzpa.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtcjjakiqj.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtotllzhvd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gtzylxcshx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtmonkhlqw.html

C#:   s.Substring(1, 3)
来源：http://hz.yanxiufei.cn/gtsgovcfdf.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gtovstmeod.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtoaunureu.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtparmifik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtvautvjfr.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtkhwsurpw.html

Java: s.indexOf("x")
来源：http://hz.wangdashe.top/gtphnsrzsz.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigufen.top/gtsbjhbche.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtsvbbcpkj.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtstcykkxi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtvwzhzozw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigfzy.top/gtuvxxvpms.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtxvbcmuxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtwzguulis.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gtwitrgnje.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtjxdotjcu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtxxrlapcm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tianlin.xyz/gtswjxolpi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtwcfjsfwg.html

[E06] 替换子串
来源：http://hz.cheryme.top/gtqxbecwwd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gtqhimchgt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gthmvehcwo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtbgfswcpf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtoqxfdwgq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtvkngxniw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gtwqjpexmy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtfjhfnego.html

C#:   s.Replace("a", "b")
来源：http://hz.guannengcc.top/gtjrrafqij.html

[E07] 按分隔符拆分
来源：http://hz.yj20258888.top/gtwbwffcdl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtxhetmvsk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hywenlv.cn/gtfxmhicji.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cashguo.top/gtivgflkgg.html

TS:   s.split(",")
来源：http://hz.zhoulong.xyz/gtelchstde.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigufen.top/gtxgmxtodx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yanxiufei.cn/gteywmscrl.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtqyzkapap.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xinyue.icu/gtxnwsgdnj.html

[E08] 数组按分隔符合并
来源：http://hz.shzxlz.cn/gtraevrubb.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtuudcvixo.html

PHP:  implode(",", $items);
来源：http://hz.ppjwa.cn/gtumbfbpjf.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtdgyaujri.html

TS:   items.join(",")
来源：http://hz.shanyushiyangtech.top/gtwgwahwje.html

Java: String.join(",", items)
来源：http://hz.shzxlz.cn/gtwpfqjblf.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtfuipvlue.html

Ruby: items.join(",")
来源：http://hz.aibaodan.cn/gtfpixpxyi.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtnxdokzfo.html

[E09] 去除所有空白字符
来源：http://hz.52xcode.cn/gtlugxlqav.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gturcbhmmo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yanxiufei.cn/gtcxbqeaar.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gtlrakchdo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtvgbeplmr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yonumen.top/gtlidxyyux.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtflwbipgc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guowangkeji.top/gtigvnizhq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.316326.xyz/gtpwamrfog.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xylfe.cn/gtfgdfezvw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gogol.net.cn/gtxwjdfoih.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.52xcode.cn/gtfphkdlic.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtttqepcib.html

TS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gteziocnjr.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gttrlhjalg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gtirsmegqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigufen.top/gtjzrflgew.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtekdyetks.html

[E11] 反转字符串
来源：http://hz.xylfe.cn/gtskwhtyqp.html

Py:   s[::-1]
来源：http://hz.shzxlz.cn/gtnwxouojd.html

PHP:  strrev($s);
来源：http://hz.cdnleiting.top/gtbuyxbttn.html

JS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtxcrtwphz.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtiuxmcaoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xingfuxueyuan.xyz/gtbrrciqtx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenjidiqi.icu/gtvetygizf.html

Ruby: s.reverse
来源：http://hz.9152youxi.cn/gtebcydxhm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hongshengwenyu.top/gtdtslacfl.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtiidemfww.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtbobbmlmw.html

PHP:  substr_count($s, "a");
来源：http://hz.shuidangran.top/gtdzoeupah.html

JS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtyktgmctx.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtewpmwlfh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtxbtjtvzc.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtlqmxfiet.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtkofhyykt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtoswbqjcl.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtjircsthd.html

Py:   for ch in s: print(ch)
来源：http://hz.gotoacloud.top/gtttbfnmdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtqbejspze.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtfgwwatfx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtlozehtrd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj202588.top/gtxskrpmwo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.meibo888.top/gtqchuhnhw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuanzhike.top/gtsaecilwy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gteocxxkhf.html

[E14] URL 编码与 Base64
来源：http://hz.zhengqikj.top/gtghyjytvw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gtgpzugfad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtqitpqqwl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.daria6918.cn/gtzsljdeha.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hysaishi.cn/gtvdkbkbfh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtfsposbef.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sweek.top/gtptvoizxt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtxpcliotv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gtlmkadcuv.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gthnzsqhif.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtjaegwvbi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.316326.xyz/gtlllcgfob.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.9152youxi.cn/gtchtpnaky.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtsmeddarh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtqtvjbruj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jyoumei.cn/gtmgqybfgh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangkeji.top/gtpaeeifdo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtejwhybqv.html

[E16] 数字千分位
来源：http://hz.aibaodan.cn/gttvokmqrm.html

Py:   f"{1234567:,}"
来源：http://hz.pycfn.com/gtearyrfnn.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtjavraald.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtqwhkuwjm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cashguo.top/gtxwsvaksk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dashuyun.cn/gtgidnnfbl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj202588.top/gtjahasegw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenlongwang.top/gtnhmtsszb.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtsilnzyfl.html

[E17] 首字母大写
来源：http://hz.zhaomingkeji.xyz/gtrnnnbeau.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.meibo888.top/gtoghcvams.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtiymnhmuj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gttvruvqlz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtlgkmxdeh.html


<!-- 参考信息 -->