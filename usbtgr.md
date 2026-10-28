代发 wailian999

C#:   list.Reverse();
来源：http://hz.meibo888.top/gtzuzkoyvx.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtanfjaqos.html

Py:   arr.index(x);  x in arr
来源：http://hz.shangyingyoupin.top/gtxmndnbry.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtlrteksqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtinjnyfte.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtsivtrwoe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.birdmap.top/gtbsbdjfrf.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gtyqtcflfy.html

Ruby: arr.index(x)
来源：http://hz.xziqi.cn/gtzfqmjgmt.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gtyajcmrjr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tianlin.xyz/gtwfilpnvj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sweek.top/gtobyzjcjx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtcxsaoeyw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtodaqoqpj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtsknpzgux.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtajuwskhb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtfaqxvrgl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgufenzy.top/gtaduydprr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtlsdsebdw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.redwolf501.top/gtjjzkbjjj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aibaodan.cn/gttovgknep.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zycfv.cn/gtenrxetdv.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtblfmopna.html

TS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtjtqnoxfx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hysaishi.cn/gtqkloeaew.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtrqpqmfnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtwaqzsmow.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shuidangran.top/gtchcqgute.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtwehvuhlb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhijiandao.cn/gtjtaduvoy.html

PHP:  array_unique($arr);
来源：http://hz.haohaochexian.top/gtdzmobiqz.html

JS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtishfunvy.html

TS:   [...new Set(arr)]
来源：http://hz.tanke756.top/gtpfwzbxhj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yuxming.cn/gtrqldahcv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtxkppbeqa.html

Ruby: arr.uniq
来源：http://hz.wangdashe.top/gttgphwajk.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtooyiuyzs.html

[D16] 求和与平均值
来源：http://hz.nanxuanxn.top/gtjudqancg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtdeszwdlb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuetiantiany.cn/gtitwzznkg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtvqlnxkuz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtbdutvmts.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gtvcwmnxyx.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gtpalspqwg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gtmcwvwtnv.html

C#:   list.Sum();  list.Average()
来源：http://hz.dianchejie.cn/gthlhbfrbe.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtwwfneity.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtnjsggzlm.html

PHP:  max($arr);  min($arr);
来源：http://hz.yangfankeji.com/gtsuykibon.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtdkpxvksj.html

TS:   Math.max(...arr);
来源：http://hz.chenjidiqi.icu/gthfjpblnv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtctczgnhy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hongshengwenyu.top/gtbafawzzb.html

Ruby: arr.max;  arr.min
来源：http://hz.guannengcc.top/gtbcvzqxas.html

C#:   list.Max();  list.Min()
来源：http://hz.aibaodan.cn/gtrctvysnv.html

[D18] 扁平化嵌套数组
来源：http://hz.xylfe.cn/gtdqtsmxgx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.haohaochexian.top/gtibkxcozx.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtxojomphw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yuxming.cn/gtycnagbpv.html

TS:   nested.flat();
来源：http://hz.guannengcc.top/gtoojlvgay.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenjidiqi.icu/gthqrkkfby.html

Go:   // 手写双层循环
来源：http://hz.hfpthk.cn/gtpdfbjjao.html

Ruby: nested.flatten
来源：http://hz.c1oappe.top/gtxtiqqfym.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guannengcc.top/gtxhzuvbvx.html

[D19] 按字段分组
来源：http://hz.daxiang520.top/gtbopkmkur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shzxlz.cn/gtajdfgvdh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zdqjudy.top/gtlexvlhoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj202588.top/gtuovksahd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuanzhike.top/gtqtvqzeqq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydjk.org.cn/gtzcnvmkar.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gtaoyrikgf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.0kj1m.cn/gtuvgryttf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtlxkshocx.html

[D20] 统计每个元素出现次数
来源：http://hz.sufxvd.cn/gtnlamhtss.html

Py:   Counter(arr)
来源：http://hz.andypj.xyz/gtrusfuzzr.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtmxwatell.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtqloippgb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jiagoushi.top/gtrvexmeuf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtnghpqasi.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtulyrsdhq.html

Ruby: arr.tally
来源：http://hz.xuetiantiany.cn/gtmfurlcts.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtcueommky.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtvdycnpzq.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gthtglnprw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.feifeiyinyue.top/gtdckhvvwn.html

JS:   arr.includes(x)
来源：http://hz.wangdashe.top/gtcnwnlopn.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtfnvaorgu.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gttuhvmyvf.html

Go:   slices.Contains(arr, x)
来源：http://hz.quarkkingdee.top/gthzpvaaph.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtgaobegae.html

C#:   list.Contains(x)
来源：http://hz.ywan-chungtsiang.top/gtrtomdjwe.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xinyue.icu/gtffzrjymd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtwojqschl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtjuvytsqh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtqypyeniy.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtfblnndhz.html

Java: new ArrayList<>(list);
来源：http://hz.mhx1999.top/gtyrwfjcdi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtuttinvsg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuanzhike.top/gtbprtnakp.html

C#:   new List<int>(list);
来源：http://hz.cheryme.top/gtqwpsvsjp.html

[D23] reduce 累积计算
来源：http://hz.hnqzz.top/gtucjfujup.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtcqbmvysa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtstcrgfzd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtnnycviny.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtiovgorob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtcebtpcwx.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtceavdubm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigufen.top/gtqlxysrbc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtkcjushkk.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydzc1.top/gtxjysfika.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtgbzvfmcf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gtazfnsedu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtoatdhfdj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtudtcvqzq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jlsjyb.cn/gttdfsijxp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtrmknhboz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gtocxipwha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nwbrower.top/gtmmohezvd.html

[D25] Set 集合去重与交并差
来源：http://hz.hammf.cn/gtmvokrurb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.mhx1999.top/gtqfmhjyzp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fengsongda.top/gtdhxilakt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hysaishi.cn/gtkzudrmjc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gtxvgkegux.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtebgqswqv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yuanzhike.top/gtcjmwhvad.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtqdevbthu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtqunkcydt.html

[D26] 数组转字符串
来源：http://hz.aibaodan.cn/gtjluxjmnr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yueranfly.top/gtgvmjyihn.html

PHP:  implode(", ", $arr);
来源：http://hz.jinghuilouyu.cn/gtqajhsfvv.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gttqrahbmq.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtaovqubrz.html

Java: String.join(", ", list)
来源：http://hz.cqqwz.cn/gtqihgqqpt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gtriiuttdt.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtjnepzhth.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gttnwihgfn.html

================================================================================
来源：http://hz.ppjwa.cn/gtkmlvteki.html

E. 字符串处理
来源：http://hz.redwolf501.top/gtqqjwavtt.html

================================================================================
来源：http://hz.bjfxy.top/gttcuddyzg.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtrlocjpjc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtnrpatmvy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtgvbzrlax.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gterhbxcsz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtueadvaat.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sysykeji.top/gttcypoiev.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenlongwang.top/gtostehysa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cdnleiting.top/gtiolbxnhb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guannengcc.top/gtobwgavvi.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtdqvxrdrw.html

Py:   "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtmwqhbehz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhoulong.xyz/gthgldgtlz.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtfecytfpu.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtiwroiujy.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtmqmjwhzx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fzhhl.top/gtxxwxigwo.html

Ruby: "ab" * 3
来源：http://hz.zhijiandao.cn/gtsmcnhemu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fengsongda.top/gtyxxrxtyg.html

[E03] 截取子串
来源：http://hz.svipenyu.cn/gtflhskdez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hysaishi.cn/gtueuhvcma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.andypj.xyz/gtsnhzuzne.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtivuncpol.html

TS:   s.slice(1, 4)
来源：http://hz.fengsongda.top/gtatjifyni.html

Java: s.substring(1, 4)
来源：http://hz.sysykeji.top/gtyruzzwjb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dianchejie.cn/gtskbyjole.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ybcxt.top/gtufauwuup.html

C#:   s.Substring(1, 3)
来源：http://hz.52xcode.cn/gtdsidzgbs.html

[E04] 查找子串位置
来源：http://hz.tian-w.cn/gtjoddviyc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtruoozckz.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gthgzjhqjh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtqibaamvu.html

TS:   s.indexOf("x")
来源：http://hz.daxiang520.top/gtiijxwthz.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gttiahbzvx.html

Go:   strings.Index(s, "x")
来源：http://hz.hnqzz.top/gtcarifijn.html

Ruby: s.index("x")
来源：http://hz.zdqjudy.top/gtynojavaa.html

C#:   s.IndexOf("x")
来源：http://hz.9152youxi.cn/gtecezkaqm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenzaomai.com/gtzsirfusu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtfdzovbbz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dianchejie.cn/gtktkybhel.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtictucxmx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xziqi.cn/gtnxgaywnx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yanxiufei.cn/gtcuazbies.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gtnzoyutpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.andypj.xyz/gtwhpbmkki.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.c1oappe.top/gtkkpnkfko.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtuqcghilz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gaohongyu789.top/gtfyaeptmp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gteleuvmop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtpedaypyw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtrljiljot.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.daxiang520.top/gtntspymjx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydzc1.top/gtvafiukbo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hfpthk.cn/gtijupsxza.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtppvhdfgi.html

[E07] 按分隔符拆分
来源：http://hz.aibaodan.cn/gtdnlgwydn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.svipenyu.cn/gtzfjskpej.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shangyingyoupin.top/gtiqnvgnxk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ywan-chungtsiang.top/gttpdiprrm.html

TS:   s.split(",")
来源：http://hz.haohaochexian.top/gttjebigvt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yvedp.cn/gtgrsynllm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtxpyolkxx.html

Ruby: s.split(",");  s.split
来源：http://hz.havefunace.top/gtvjemxhdm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtrpifolnu.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtovuvtado.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtqvkijrcq.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtmbatdipf.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gttvzynayo.html

TS:   items.join(",")
来源：http://hz.yangfankeji.com/gtvutaoefa.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtwgwmunaf.html

Go:   strings.Join(items, ",")
来源：http://hz.xuetiantiany.cn/gtlidggulp.html

Ruby: items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtrrwbrkkj.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtqekksqok.html

[E09] 去除所有空白字符
来源：http://hz.snrcjt.cn/gttwsrqthq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jianghu66.top/gtpcgppjnn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hysaishi.cn/gtvidangfn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zdqjudy.top/gteypjjhhj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtvbnuicxf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.kuanghao11.cn/gtxtbsriug.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangdashe.top/gtwuwmgwfd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jiagoushi.top/gtsscpchxx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.bjfxy.top/gtrxbhoycd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ywan-chungtsiang.top/gtesjkzeir.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.quarkkingdee.top/gtvxyidjls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtlcuzyfuo.html

JS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtnmujjoif.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtmksajzwh.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtfmezojwy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aibaodan.cn/gtxemlysqp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gtrksloxyg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gtgrcmefwt.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtzfcaczey.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtqzvosnlq.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtjibsnedr.html

JS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtlsenkafz.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gthmzgbmte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhaomingkeji.xyz/gtxtajujxl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnqzz.top/gtgiwfouxx.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtskrsmtjl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuanzhike.top/gtzgwrmpeq.html

[E12] 统计某字符出现次数
来源：http://hz.cdnleiting.top/gtmuenwulr.html

Py:   s.count("a")
来源：http://hz.cucudq.cn/gttddesqzb.html

PHP:  substr_count($s, "a");
来源：http://hz.hongshengwenyu.top/gtffwehslu.html

JS:   s.split("a").length - 1
来源：http://hz.shzxlz.cn/gtfycckrvp.html

TS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtthbdlvey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtuqdxxaze.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gtozgnfzwm.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtyghmnhvy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aizwys.cn/gtynwxinhc.html

[E13] 逐字符遍历
来源：http://hz.xziqi.cn/gtgoelkqul.html

Py:   for ch in s: print(ch)
来源：http://hz.yonumen.top/gtgmqnvsjp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gtdzslqtpt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gogol.net.cn/gtkhfeisuo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtmrdijqde.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtgjdvrypa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtqihcosyq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xziqi.cn/gtmjzsyhub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gtnfdcpzkn.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtupqwkknr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sufxvd.cn/gtbzbzblrs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtnxqualsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.havefunace.top/gtnhaguoum.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtonovmepz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sxryk.cn/gtiszepxti.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtppuntigr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shzxlz.cn/gtiszfgjyc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.havefunace.top/gtfovmqvgh.html

[E15] HTML 转义 / 反转义
来源：http://hz.c1oappe.top/gtnmtkmlaj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tanke756.top/gtpseagtif.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gtseesyrgo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuetiantiany.cn/gtqvodizgq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.nanxinkj.top/gtixldxzrr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.pycfn.com/gtgvajdddw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtxflmjvgg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuxming.cn/gtujgfvylt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtfpelstkk.html

[E16] 数字千分位
来源：http://hz.sxryk.cn/gtgmdbixkg.html

Py:   f"{1234567:,}"
来源：http://hz.sweek.top/gtewahdmfj.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtvyobpzky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtafzfpeyi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jiagoushi.top/gtrkkjmbeu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgfzy.top/gtosmfoyeq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuanzx.com/gtmbwiiufk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtwgnqhzhk.html

C#:   1234567.ToString("N0")
来源：http://hz.chenjidiqi.icu/gtlparzrqv.html

[E17] 首字母大写
来源：http://hz.hnqzz.top/gtznwxpavm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yangfankeji.com/gtkuihrqoj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtchjudohz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtjpllhjrt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtrolznofe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gtxgrlkiif.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtfgipoqrm.html

Ruby: s.capitalize
来源：http://hz.cashguo.top/gtqjtdmriz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtoarorsbu.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtbygbgrwp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtmrlfxyng.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yonumen.top/gtiwrdglec.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtudpjytya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtstsswlzx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ehwqpu.com/gtgchoewqs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xinyue.icu/gtjgmjtest.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhiwuduotai.top/gtekkrqmgg.html


<!-- 参考信息 -->