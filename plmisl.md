代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtgyayfzml.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtqbfcskkf.html

Go:   slices.Reverse(arr)
来源：http://hz.fengsongda.top/gtbviqupil.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtabkmfdua.html

C#:   list.Reverse();
来源：http://hz.yj202588.top/gtuupmxcht.html

[D12] 查找元素下标
来源：http://hz.sxryk.cn/gtujwljhch.html

Py:   arr.index(x);  x in arr
来源：http://hz.hfpthk.cn/gtzukdhiod.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtaczupuam.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtxdmnshsp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gthfpjsezp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtaxqzyxxk.html

Go:   slices.Index(arr, x)
来源：http://hz.feifeiyinyue.top/gtobpakqab.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtuxerazyv.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtfxnjxgph.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tanke756.top/gtgujveqcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xinyue.icu/gtmeghyppc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtshxoyjbo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtztidsdhj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtvwahsdsy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydjk.org.cn/gtqbyjlmeh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.feifeiyinyue.top/gtpfenyemp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnqzz.top/gthrrzwrbk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.vqdsnc.cn/gtpukxxypv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.vqdsnc.cn/gtokesqtlw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhoulong.xyz/gtpiwuaegi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shuidangran.top/gttvykhayd.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtwcdlkhes.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtpkrbtwrc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxuanxn.top/gtmsidizrv.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtewabhmme.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.dashuyun.cn/gtcpusbjfy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pycfn.com/gtpqffpzzy.html

[D15] 去重
来源：http://hz.jyoumei.cn/gtogbgtefv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gttneqoupv.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gtabvaawlf.html

JS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtdpzkercx.html

TS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtzppuykwe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj202588.top/gtrtloprns.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtlgowmnwa.html

Ruby: arr.uniq
来源：http://hz.zhijiandao.cn/gteviimiue.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gtomqegtux.html

[D16] 求和与平均值
来源：http://hz.redwolf501.top/gttjdxljwk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shuidangran.top/gtnmdopmif.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtoolvoquv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtmheqtohw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenlongwang.top/gthihvptsn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtyftkltjl.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtlhspxfsx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.tanke756.top/gtrqooybqe.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtnxdxqzfr.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtlhwwjljx.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtgvrdtztp.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtasoptjdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guannengcc.top/gtthzygyqk.html

TS:   Math.max(...arr);
来源：http://hz.jinqigfzy.top/gtjnkyqxaw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtlqnhragk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gtvhbjhpnu.html

Ruby: arr.max;  arr.min
来源：http://hz.pengpengdd.cyou/gthpyvmdko.html

C#:   list.Max();  list.Min()
来源：http://hz.hnxiangtu.top/gtwhtyrzdi.html

[D18] 扁平化嵌套数组
来源：http://hz.zdqjudy.top/gtptszwvon.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hammf.cn/gtogybzhrj.html

PHP:  array_merge(...$nested);
来源：http://hz.gotoacloud.top/gtmpyvvaic.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.redwolf501.top/gtvedqqhuc.html

TS:   nested.flat();
来源：http://hz.guowangkeji.top/gthwyftuzm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aizwys.cn/gtdjtomqew.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtbxogcvlh.html

Ruby: nested.flatten
来源：http://hz.hysaishi.cn/gtlvbhqzoi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtlgwgrsod.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtjybczcmh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ybcxt.top/gtonepwkhc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jlsjyb.cn/gtruyhpdyn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtelriwiyv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtpkvtzqcl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.bjfxy.top/gttsrhkvdd.html

Go:   // 手写 map[string][]T
来源：http://hz.hongshengwenyu.top/gtiosievnm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zdqjudy.top/gtbaaruowl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtyzzretrd.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gtpxpqaqiq.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtxpuiyutf.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtvwxswdut.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtfgkvxgoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtyfgtrwnx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yongpay.top/gttfjfyzmf.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gttcduretx.html

Ruby: arr.tally
来源：http://hz.xuanzx.com/gtvnmphzre.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenzaomai.com/gtrghwygmm.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtodapyoul.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtmwilypuj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtwtnwlpcs.html

JS:   arr.includes(x)
来源：http://hz.havefunace.top/gteexwtxjc.html

TS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtlxymskwb.html

Java: list.contains(x)
来源：http://hz.hysaishi.cn/gtwqlbbycv.html

Go:   slices.Contains(arr, x)
来源：http://hz.daxiang520.top/gtuexqnbpt.html

Ruby: arr.include?(x)
来源：http://hz.yvedp.cn/gthvvirqqe.html

C#:   list.Contains(x)
来源：http://hz.kuanghao11.cn/gtiazsurtk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtkdsceyyf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtgnkwoivc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.guowangkeji.top/gtmzestooo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.haohaochexian.top/gtesgpxetr.html

TS:   [...arr];
来源：http://hz.0kj1m.cn/gtshkbdygj.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtvcpwzcew.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtkspagpuq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hywenlv.cn/gtmqgdkooe.html

C#:   new List<int>(list);
来源：http://hz.vqdsnc.cn/gtheuqkktm.html

[D23] reduce 累积计算
来源：http://hz.ywan-chungtsiang.top/gtrzmfbsld.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.meibo888.top/gtxfxpuvao.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtobawceqm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gthjenaoht.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gttqlokxwf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gtfdrsyvhg.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtetvwvcie.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shangyingyoupin.top/gtxsmyueoo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hywenlv.cn/gtlocwcloq.html

[D24] 字典 / Map 基本操作
来源：http://hz.yueranfly.top/gtjedndlfg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tanke756.top/gtjguxejif.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangshuangyany.cn/gtcefesnpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtxagqcgon.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gaohongyu789.top/gtcaxiardw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shangyingyoupin.top/gthweugvmd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hammf.cn/gtsceqdfxb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhengqikj.top/gthfdpijtb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sufxvd.cn/gtcjmgesfl.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtaxnokwlk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tanke756.top/gtpermfllm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtpvdahwnh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinghuilouyu.cn/gthtcfepzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydzc1.top/gtplehvpig.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtbaqmtkea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtkplaqraj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cashguo.top/gtnklhjwus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtclemyuxp.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtkvysjeqv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gzhubu.top/gtskpuoqsx.html

PHP:  implode(", ", $arr);
来源：http://hz.vqdsnc.cn/gtsjpqgjbc.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtqpjxwkfl.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtzgkndhib.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtyjebdezm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtukjanlgb.html

Ruby: arr.join(", ")
来源：http://hz.zhongyouzk.top/gtuyxtegdr.html

C#:   string.Join(", ", list)
来源：http://hz.ybcxt.top/gtbocudwhq.html

================================================================================
来源：http://hz.cqqwz.cn/gtuwifflec.html

E. 字符串处理
来源：http://hz.meibo888.top/gtpcwmilwl.html

================================================================================
来源：http://hz.yvedp.cn/gtvwgksuar.html

[E01] 拼接字符串
来源：http://hz.iojbl.cn/gtbfxylbtr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yonumen.top/gtfsetxjvi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hammf.cn/gtsptjoapj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtlorajrrk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtxtfjuopz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtiselprnr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sufxvd.cn/gtqowxttsy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtiqsaskqc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gthdcsnbbp.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtdftcvwvx.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtwdobfmsh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtgrsqkfbz.html

JS:   "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtjuunmowl.html

TS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtnixzbbid.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtxclfprcy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnqzz.top/gttdobmafe.html

Ruby: "ab" * 3
来源：http://hz.nwbrower.top/gtmtejwigx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtlmhympcg.html

[E03] 截取子串
来源：http://hz.gaohongyu789.top/gtwpdjqihe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nanxuanxn.top/gtjmivwrdv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guannengcc.top/gtqxmnnqee.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtpxqagrba.html

TS:   s.slice(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtlejgqsgo.html

Java: s.substring(1, 4)
来源：http://hz.jianghu66.top/gtzltxhbpd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtndywvgis.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gtnaugsjax.html

C#:   s.Substring(1, 3)
来源：http://hz.gzhubu.top/gtxlmtypwk.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtmaixdwpt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgufenzy.top/gtewzezcpo.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtorebftwg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgufenzy.top/gtnzggnfaa.html

TS:   s.indexOf("x")
来源：http://hz.ppjwa.cn/gthszaohbk.html

Java: s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtydbutffu.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gtttybgbay.html

Ruby: s.index("x")
来源：http://hz.meibo888.top/gtisuflyiv.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtgzkokiys.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gtmimwzvfm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zycfv.cn/gtmxuxulln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tianlin.xyz/gtkrxillqm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtkeesyuen.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtreaivhcu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtjyjkprwt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jianghu66.top/gtwsdszhhm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.kuanghao11.cn/gtrslhtozb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj202588.top/gtghrcujnj.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtmwcarpgq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtacdzzvni.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sxryk.cn/gthbmbdaoc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtnwfuhtch.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtkwquvnhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtdoqcxvgj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.smart0.xyz/gtekoalyml.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtineoucod.html

C#:   s.Replace("a", "b")
来源：http://hz.sufxvd.cn/gtizfqgigm.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gtetkltqhh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.havefunace.top/gtnamgoanf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gaohongyu789.top/gtvcpxkfci.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtbdzockrh.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtphbpguxu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shzxlz.cn/gtscjjnhve.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yueranfly.top/gtwpmpcawb.html

Ruby: s.split(",");  s.split
来源：http://hz.fzhhl.top/gtygikxjrc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtojpgbdno.html

[E08] 数组按分隔符合并
来源：http://hz.hammf.cn/gtidzrnwtb.html

Py:   ",".join(items)
来源：http://hz.hysaishi.cn/gtcddnlqer.html

PHP:  implode(",", $items);
来源：http://hz.jiagoushi.top/gtmjrcogtz.html

JS:   items.join(",")
来源：http://hz.sxryk.cn/gtrbzevzhq.html

TS:   items.join(",")
来源：http://hz.jyoumei.cn/gtnkktiqhf.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtxdclrkce.html

Go:   strings.Join(items, ",")
来源：http://hz.sysykeji.top/gtfkcmpyan.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtohwxwntp.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtpucsmqnu.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtzycifboh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtvlrhqbbx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtlmnotgef.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtoilccnwo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtzfhibmvw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.guowangkeji.top/gtboqbmmzq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jinghuilouyu.cn/gttdmohhki.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.iojbl.cn/gtzcojllkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pengpengdd.cyou/gtcrhslddx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtxxaanjel.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtzrrtvgwo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangdashe.top/gteufzwgjz.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtlvqtdxui.html

TS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtgujidovx.html

Java: String.format("%03d", 7)
来源：http://hz.yangfankeji.com/gtvvpzlmbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tanke756.top/gtvtniopmy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhengqikj.top/gtrsoatwcz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtzscwtfpv.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtwzdfcarq.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtxbochjke.html

PHP:  strrev($s);
来源：http://hz.0kj1m.cn/gtzikbhggo.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtbapqqbrk.html

TS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtruihymbl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.andypj.xyz/gtlbcltmvn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtkrcgbqxi.html

Ruby: s.reverse
来源：http://hz.hammf.cn/gtdhmlokfp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.guowangkeji.top/gtwnvixtkv.html

[E12] 统计某字符出现次数
来源：http://hz.cqqwz.cn/gtwxuxocxx.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gtbzqthwvk.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtfmkcasde.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtcbuaskmr.html

TS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtuhqtofqj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtmvuiaznw.html

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtejpvbgqu.html

Ruby: s.count("a")
来源：http://hz.zhixingplan.top/gtyqmatcgl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gttfynkcte.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gtysmwvegi.html

Py:   for ch in s: print(ch)
来源：http://hz.redwolf501.top/gtuzsectyi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxuanxn.top/gtrsjqpibp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtntkbqgir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtlzmtupms.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hywenlv.cn/gtwzjakewm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtxiwjqtlr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtsnfbsfpx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guowangkeji.top/gtkaxtcnfg.html

[E14] URL 编码与 Base64
来源：http://hz.gogol.net.cn/gticpyxpwd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtyvgrhjcl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.9152youxi.cn/gtntwxssft.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ydjk.org.cn/gtbobyjgxv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtyxfygizv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtitqegigf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtrsodfowe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gzhubu.top/gtaqwpzxvz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guannengcc.top/gtgbnxjlgb.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj202588.top/gtcmedqurk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gthrbxuocq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sysykeji.top/gtegmtwojb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gthpevdzhh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tian-w.cn/gtpcuctbxd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtfpryfbjc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yvedp.cn/gtilscrquz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yongpay.top/gtfdirlkrh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cqqwz.cn/gttvhjgzqn.html

[E16] 数字千分位
来源：http://hz.yangfankeji.com/gtenzuhjyz.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtmdvilnjx.html

PHP:  number_format(1234567);
来源：http://hz.yj20258.top/gtingshlxv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtneipknfb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtgibasrcm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yueranfly.top/gtqpafgkil.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtyybhufez.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtwfshbmeu.html

C#:   1234567.ToString("N0")
来源：http://hz.yangfankeji.com/gtkisjingy.html

[E17] 首字母大写
来源：http://hz.quarkkingdee.top/gtbqiauouy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtukykebcy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtjioyfmov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtcqnltbag.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtezvgxran.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shuidangran.top/gtlrulrfft.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tianlin.xyz/gtclzorolk.html

Ruby: s.capitalize
来源：http://hz.xziqi.cn/gtnrbqgfdx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xylfe.cn/gtirkjshde.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtlvbbtien.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhijiandao.cn/gtcdnfpkea.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtbyswsuqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtkqzwdncn.html


<!-- 参考信息 -->