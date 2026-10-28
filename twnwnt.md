代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtvlkbwmtp.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtceopgmew.html

Go:   slices.Reverse(arr)
来源：http://hz.hnxiangtu.top/gtnnrsiqao.html

Ruby: arr.reverse
来源：http://hz.quarkkingdee.top/gthnfzwqtk.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtnpdxhfpo.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtepspfpti.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnxiangtu.top/gtmryqfsgu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hysaishi.cn/gtarukdyir.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gtnmlxbbyb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtfhqksskm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jqgfzy.top/gttfiffyoh.html

Go:   slices.Index(arr, x)
来源：http://hz.aizwys.cn/gtkxmgyirw.html

Ruby: arr.index(x)
来源：http://hz.yvedp.cn/gtpcatpyck.html

C#:   list.IndexOf(x);
来源：http://hz.chenjidiqi.icu/gtrnpggpar.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xinyue.icu/gtalivdwlp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gttqyrohnt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.9152youxi.cn/gtglmiesyz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtevgmmshv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cashguo.top/gtrjcvfhqv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ivvv.top/gtejrvgotr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtkjcsiqur.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.316326.xyz/gtnedrqldo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.nanxuanxn.top/gtaqrkzmdq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtdbkkmlpi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aibaodan.cn/gtloeqklla.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtmvwxxlwc.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtkvliczog.html

TS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtysfgeolf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtpkjphkvr.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtsxfagzzg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtvqfaalwj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtwqndiohc.html

[D15] 去重
来源：http://hz.chenzaomai.com/gtdvpngmox.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtryykuwxb.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtsajyeqaa.html

JS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtwrbrvnyk.html

TS:   [...new Set(arr)]
来源：http://hz.dashuyun.cn/gtlekagxzr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.guowangkeji.top/gtgxqvnwrn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gaohongyu789.top/gtejgjxqpt.html

Ruby: arr.uniq
来源：http://hz.yonumen.top/gtgssqxiwm.html

C#:   list.Distinct().ToList()
来源：http://hz.feifeiyinyue.top/gtzffnkuiq.html

[D16] 求和与平均值
来源：http://hz.ppjwa.cn/gtcghteieg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.snrcjt.cn/gtikvpthaw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtpwtlfsso.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigufen.top/gtxpazulqi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daria6918.cn/gtthyjvebl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gtobecrkil.html

Go:   // 手写循环累加
来源：http://hz.andypj.xyz/gtypzmkoel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtrwejaanz.html

C#:   list.Sum();  list.Average()
来源：http://hz.ehwqpu.com/gtwqnqrywt.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtjyvmzqyy.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtmgparsro.html

PHP:  max($arr);  min($arr);
来源：http://hz.gogol.net.cn/gtrwkgrcxl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtlpebweqx.html

TS:   Math.max(...arr);
来源：http://hz.smart0.xyz/gtghrnldha.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gttjotrszj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtonfmbuef.html

Ruby: arr.max;  arr.min
来源：http://hz.smart0.xyz/gtkencbffk.html

C#:   list.Max();  list.Min()
来源：http://hz.chenjidiqi.icu/gtexolfkru.html

[D18] 扁平化嵌套数组
来源：http://hz.daria6918.cn/gtuowwkgaj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtooczukax.html

PHP:  array_merge(...$nested);
来源：http://hz.ydzc1.top/gtmifdomhz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gtjnehltbs.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtbptxwnad.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.havefunace.top/gtyjgdeomq.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtolgtdisp.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtoxogbvdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenlongwang.top/gtklwhfvyj.html

[D19] 按字段分组
来源：http://hz.pycfn.com/gtavimxoec.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gtqofgauam.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.52xcode.cn/gtoobihvwu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhaomingkeji.xyz/gtpnfrxpch.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xuanzx.com/gtotpdbdqd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtcmrjnjkm.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gtrbkwzciy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtnmjtnksa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtewvxfmhe.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtuccgbjkx.html

Py:   Counter(arr)
来源：http://hz.chenlongwang.top/gtpsmogxxu.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigfzy.top/gtvxlnmuqe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtmpviqwuu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtfhkxrjfi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtpgdfiqbm.html

Go:   // 手写 map[T]int
来源：http://hz.c1oappe.top/gtzeygfwci.html

Ruby: arr.tally
来源：http://hz.shangyingyoupin.top/gtpobeejqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtlpvklamr.html

[D21] 判断是否包含某元素
来源：http://hz.yangfankeji.com/gttlsplyly.html

Py:   x in arr
来源：http://hz.fzhhl.top/gtkkfniflt.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hysaishi.cn/gtsecvbznm.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtvyajqngr.html

TS:   arr.includes(x)
来源：http://hz.hywenlv.cn/gtvbphhypf.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtwciyreuy.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gttmbamtnl.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtlecbyjyu.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtepagwneq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtnopxuxtk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zycfv.cn/gtomliarhq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gttruypcbs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258888.top/gtivoghzqq.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtcshjibzx.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtejweyqzb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gtdtztjtvb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenzaomai.com/gtkilaunzm.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gthsbtkoci.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gteywlureh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.316326.xyz/gtolqyutwr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hfpthk.cn/gtyagvthho.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtfijzrytv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhongyouzk.top/gtwgrstqsy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtcgwqgnrr.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gtzgrbbaci.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtrdbppige.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtehwsiuow.html

[D24] 字典 / Map 基本操作
来源：http://hz.aizwys.cn/gttbdxekcb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gthzibkxwz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jyoumei.cn/gtolvomnbb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.iojbl.cn/gtufvfyxuf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gotoacloud.top/gtzdfdrrwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtnwlcvpgi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gthhcngzlc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gtujkwyryf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtfnjoltzt.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtnyrrmaut.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jianghu66.top/gtyinjloyh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtfgvmdxgu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtxwqoaxqy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtqixbtvns.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtzgecfsyd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gthcgnkqii.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xziqi.cn/gtgperouie.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhengqikj.top/gtgwbhfnyp.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtdobvyyfu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtxdnchbnr.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgufenzy.top/gtxtdlrsfc.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtbfzancxg.html

TS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtjjwgbbqy.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtgkjpzjle.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ybcxt.top/gtfjwjdbun.html

Ruby: arr.join(", ")
来源：http://hz.redwolf501.top/gtdfvmrljc.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gtxqdvdhwk.html

================================================================================
来源：http://hz.andypj.xyz/gtpgqgmwsi.html

E. 字符串处理
来源：http://hz.bjfxy.top/gthznswkmt.html

================================================================================
来源：http://hz.yj20258.top/gtgzimftxy.html

[E01] 拼接字符串
来源：http://hz.cashguo.top/gtrotqeooi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtfcvmzioy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gotoacloud.top/gttnwxctje.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtfuqrihsk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtzrrdpkyl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtaxrnsavy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtnhzxnkrm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gtnidadini.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.fzhhl.top/gtcawfvkdh.html

[E02] 重复字符串
来源：http://hz.cashguo.top/gtakfxhvru.html

Py:   "ab" * 3
来源：http://hz.sysykeji.top/gtescricyx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigfzy.top/gtrqpxdoaa.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gttljlrasy.html

TS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtlkjfsvla.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtphnfipff.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtqqxfkzhr.html

Ruby: "ab" * 3
来源：http://hz.52xcode.cn/gtoobtivpu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cdnleiting.top/gtrldtxvvj.html

[E03] 截取子串
来源：http://hz.hywenlv.cn/gtcjbsmrma.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtqxsjoshh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sysykeji.top/gtjdvduxbh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtyqeeifcp.html

TS:   s.slice(1, 4)
来源：http://hz.hongshengwenyu.top/gtepikxisd.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gtpteholfi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtdhbyxhzo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhongyouzk.top/gtqtrukdfw.html

C#:   s.Substring(1, 3)
来源：http://hz.smart0.xyz/gtcpixhfre.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtayvsfggu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daxiang520.top/gtkmyphjee.html

PHP:  strpos($s, "x");
来源：http://hz.cucudq.cn/gtcskdjotg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtqtzyjsqj.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtkwpybdzw.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtiexpmqzg.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtriqzjgzb.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtaydxhcci.html

C#:   s.IndexOf("x")
来源：http://hz.hysaishi.cn/gtkkfjbmvk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxinkj.top/gtugexvxtl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtakjxfftt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtewilxsca.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gthljoljji.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xinyue.icu/gtwfncxssz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtbqldsfsn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gtabtyawng.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtdodiwuwf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ywan-chungtsiang.top/gtxnatksdu.html

[E06] 替换子串
来源：http://hz.xinyue.icu/gtnmkegmpj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.0kj1m.cn/gtgpokzsqb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ybcxt.top/gtsyoxizwj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtrlcojzja.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtbavessuh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxuanxn.top/gtjvihhner.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.bjfxy.top/gtysrptdxl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnxiangtu.top/gtpixeldhm.html

C#:   s.Replace("a", "b")
来源：http://hz.chenjidiqi.icu/gtwrmujybu.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtnwapjnem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangtech.top/gtdoymdezx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtyysjivcw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.meibo888.top/gtexlruxby.html

TS:   s.split(",")
来源：http://hz.vqdsnc.cn/gtfxqqejkt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hfpthk.cn/gtrtehsmle.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydjk.org.cn/gtpddvqlax.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtrdqdwiqg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fengsongda.top/gtwcfrdswn.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtzdbhegph.html

Py:   ",".join(items)
来源：http://hz.hywenlv.cn/gtukzzmvgm.html

PHP:  implode(",", $items);
来源：http://hz.jianghu66.top/gtsccoilrk.html

JS:   items.join(",")
来源：http://hz.ydzc1.top/gtjyirxunn.html

TS:   items.join(",")
来源：http://hz.havefunace.top/gtwxlfkrwp.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtdnfnwpdi.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtaspeoajf.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtaxexxvyt.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtfyllrnnu.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtewhvzteg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgfzy.top/gtlnymvrtz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhongyouzk.top/gthteaypoa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtddssrtqa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gthihahand.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.smart0.xyz/gtonycdszb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hongshengwenyu.top/gtbmospabn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.c1oappe.top/gtijhubjgy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.feifeiyinyue.top/gtmoimepbr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.daxiang520.top/gttprwkphg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtjahjluwx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnxiangtu.top/gtmthxewxm.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtawsodleh.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtianszpop.html

Java: String.format("%03d", 7)
来源：http://hz.yvedp.cn/gtrxerhhdi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pycfn.com/gtqwhflajf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtdklfabco.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yj20258888.top/gtwnsrovqa.html

[E11] 反转字符串
来源：http://hz.316326.xyz/gtqjxkoccb.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtcqfssomb.html

PHP:  strrev($s);
来源：http://hz.snrcjt.cn/gtkmfggkkj.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gthtjfhpib.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtakxdvity.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtgbdhteni.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtytirtarq.html

Ruby: s.reverse
来源：http://hz.smart0.xyz/gttxinlndw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtyhbzaowd.html

[E12] 统计某字符出现次数
来源：http://hz.xylfe.cn/gtriimdapx.html

Py:   s.count("a")
来源：http://hz.yangfankeji.com/gtuqgikvir.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtnagptxfu.html

JS:   s.split("a").length - 1
来源：http://hz.yangfankeji.com/gtdedzacgq.html

TS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtapyhfcpm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pengpengdd.cyou/gtlivcaitv.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtseparesr.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtyeqzlzzp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gttdwxdtzd.html

[E13] 逐字符遍历
来源：http://hz.yuanzhike.top/gtuzratrtw.html

Py:   for ch in s: print(ch)
来源：http://hz.kuanghao11.cn/gttogfbruf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtkcpsslvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtrycacovs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gtknfulqyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gaohongyu789.top/gtggaekjun.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jlsjyb.cn/gtowrrzzvp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shuidangran.top/gtkvhvcsho.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj202588.top/gtifauvrvq.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtvxexzfng.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtguymjsnp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gteyuexsta.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.bjfxy.top/gtcilywooe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.mhx1999.top/gtdcnaodpa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtrbujfkys.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yj20258888.top/gtivcsnjkl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtiaxwtwbc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtapzrpmgl.html

[E15] HTML 转义 / 反转义
来源：http://hz.ivvv.top/gtcucdgolx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gotoacloud.top/gtcdpgvpvt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cqqwz.cn/gtyknerozw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtiasqvweo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.wangshuangyany.cn/gtqnixfyxx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.birdmap.top/gtqayxulgr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.birdmap.top/gttxhregec.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jianghu66.top/gtxqtflpwl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cucudq.cn/gtegkokwxt.html

[E16] 数字千分位
来源：http://hz.jqgfzy.top/gtoreeltgx.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtkrttcrfi.html

PHP:  number_format(1234567);
来源：http://hz.zhixingplan.top/gtxufrozei.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gthwfbxwog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtgggoonfs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gttdsmyitb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sufxvd.cn/gtyhgasofm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtkvkqzypl.html

C#:   1234567.ToString("N0")
来源：http://hz.quarkkingdee.top/gtodwclwok.html

[E17] 首字母大写
来源：http://hz.shanyushiyangkeji.top/gtkozodvwi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gthmatlzeg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtoyvpopuf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtnlcysroz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gtnhenehke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtcwefozut.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtumxjoexs.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gtorinhhah.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.zhiwuduotai.top/gtkwuaehsf.html

[E18] 模板占位符替换
来源：http://hz.ehwqpu.com/gtfdktzuvt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tanke756.top/gtznbvcgxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gogol.net.cn/gtqewzqdrz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.andypj.xyz/gttoxncwya.html


<!-- 参考信息 -->