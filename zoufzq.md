代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtsuyhvqis.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtqynezxan.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtdjaoubmd.html

Go:   slices.Index(arr, x)
来源：http://hz.guowangkeji.top/gthnpdqqlg.html

Ruby: arr.index(x)
来源：http://hz.sufxvd.cn/gtljedkabt.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtppyezhjl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenjidiqi.icu/gtxkexkuig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtidvzbzkx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtclcycbex.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtekdjlemg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtaxikhhhv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtuctypphy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guowangkeji.top/gtjpuelryl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigufen.top/gtyatcajss.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.birdmap.top/gtlfctwyjp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtilosuyzf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhaomingkeji.xyz/gtayijkhxl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cucudq.cn/gtqcxnqlgw.html

JS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtpopnwhep.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gtinwckija.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shuidangran.top/gtmsbxctvm.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gttpvghrin.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnxiangtu.top/gtljvtqayy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ehwqpu.com/gtuerflico.html

[D15] 去重
来源：http://hz.gogol.net.cn/gtoxegvlgr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.mhx1999.top/gtkuurajci.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtlselxtxv.html

JS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtofgsjgnl.html

TS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtfldlpidl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fengsongda.top/gtkwbinftv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yangfankeji.com/gtcjykgfdm.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtxkoureht.html

C#:   list.Distinct().ToList()
来源：http://hz.cheryme.top/gtkyryeclk.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtdiqioazz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jlsjyb.cn/gtqlsyztsz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhaomingkeji.xyz/gtqpxgxyib.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtdwgvvtze.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtqlcavmyq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daria6918.cn/gtbihdiabf.html

Go:   // 手写循环累加
来源：http://hz.yongpay.top/gttuklqdeu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cashguo.top/gthwomdgzl.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhixingplan.top/gtdoikgtus.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtoypiijch.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtshdfrlov.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtjvbauwrq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daria6918.cn/gtmjazoqml.html

TS:   Math.max(...arr);
来源：http://hz.zdqjudy.top/gtbldaqnki.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtcbksxxbm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.c1oappe.top/gtvbnymtgi.html

Ruby: arr.max;  arr.min
来源：http://hz.zhaomingkeji.xyz/gtqbgsrbsv.html

C#:   list.Max();  list.Min()
来源：http://hz.hysaishi.cn/gtwwwhvxso.html

[D18] 扁平化嵌套数组
来源：http://hz.hywenlv.cn/gtmzzqucge.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtbvyzpnyc.html

PHP:  array_merge(...$nested);
来源：http://hz.sxryk.cn/gtnsirohot.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtycqgfgls.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gtehmgadfa.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fzhhl.top/gtazwwktkz.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtkbhikrsg.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtdtaveemm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtqdxxrcyl.html

[D19] 按字段分组
来源：http://hz.gzhubu.top/gtpldtznpt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.feifeiyinyue.top/gtyddwrpac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gogol.net.cn/gthnkaqxsx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sxryk.cn/gtvipowwjx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtxuidsqcs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtiygpaugm.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gtnasqkrtu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtikelvdct.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.iojbl.cn/gtfwfxlaze.html

[D20] 统计每个元素出现次数
来源：http://hz.yuxming.cn/gtdmfyegsl.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtyswgvxau.html

PHP:  array_count_values($arr);
来源：http://hz.chenjidiqi.icu/gtgsdxgizn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtjnjkfotf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtkoryamvs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhaomingkeji.xyz/gtbgzffjha.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtikyjwcsm.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gthhyfvvoq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtspyqbhmp.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtczkrpewr.html

Py:   x in arr
来源：http://hz.quarkkingdee.top/gtszpcxzdr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xuanzx.com/gtmtijnmks.html

JS:   arr.includes(x)
来源：http://hz.yongpay.top/gtkabczhhz.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gthnlybtfd.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtmktgdjhp.html

Go:   slices.Contains(arr, x)
来源：http://hz.snrcjt.cn/gthdwilcex.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gttxpqqwoh.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtwrpeckqr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gtmonvhitl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtbfaycsgs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtdaelwgcs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhijiandao.cn/gtkcxndhzq.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtkwvxmghv.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtvdwpywqt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cashguo.top/gtsxwuvlyi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.316326.xyz/gttrzcmunm.html

C#:   new List<int>(list);
来源：http://hz.52xcode.cn/gtwmcfnouz.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtveogvjzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtpzsxmrjz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jlsjyb.cn/gtgbdxcpeo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtsanamfkt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtravivdop.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shanyushiyangkeji.top/gtccdgmctc.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtwhpopmzs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.redwolf501.top/gtvbisppup.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.snrcjt.cn/gtnwptmlwj.html

[D24] 字典 / Map 基本操作
来源：http://hz.shzxlz.cn/gtdskzurff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.vqdsnc.cn/gtlzwwqfvk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gtbsloctxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhijiandao.cn/gtbrdfszue.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gtzlkcjewy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gthjixffsr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtmfejudkd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtpdjefeoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ywan-chungtsiang.top/gtzaedwbjh.html

[D25] Set 集合去重与交并差
来源：http://hz.jinghuilouyu.cn/gtwhzcmvkq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtybdahyrw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtcwhhciuv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydzc1.top/gtfisyanky.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gteuxfembo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtroqrfavw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigfzy.top/gttshqgfew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tian-w.cn/gtswachglm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtqxjwaubj.html

[D26] 数组转字符串
来源：http://hz.xinyue.icu/gtudmtrznd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigfzy.top/gtuvmcfoxw.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigufen.top/gtjbjkgayo.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtrawzasza.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtiqxmoyex.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtbuusgxek.html

Go:   strings.Join(strs, ", ")
来源：http://hz.bjfxy.top/gtprjieyyg.html

Ruby: arr.join(", ")
来源：http://hz.316326.xyz/gtdglxydwe.html

C#:   string.Join(", ", list)
来源：http://hz.chenzaomai.com/gtsulpgghh.html

================================================================================
来源：http://hz.shzxlz.cn/gtzrmurfqj.html

E. 字符串处理
来源：http://hz.zycfv.cn/gtzcewfzcn.html

================================================================================
来源：http://hz.zhixingplan.top/gtbyecjxze.html

[E01] 拼接字符串
来源：http://hz.xuetiantiany.cn/gtejxelfsb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhengqikj.top/gtzzhanlrd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtwpdbzyfm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtwwwrpwgf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtxnurpoid.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnqzz.top/gtotawmjyz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtielgjzjd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtbvvdhqqv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuanzhike.top/gtugtsbhjj.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtiktdoywo.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtqsfluxxs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtkmjlnfsf.html

JS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gtmqeswsyx.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gthvykohfx.html

Java: "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtvirpiwro.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhixingplan.top/gtitnetifb.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtqqfxgwou.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hammf.cn/gtpgkdyxhv.html

[E03] 截取子串
来源：http://hz.daxiang520.top/gtpfkdkfvr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gttzvjfykx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtknzwlrdw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtkfkflzjd.html

TS:   s.slice(1, 4)
来源：http://hz.yonumen.top/gtgrfyaauj.html

Java: s.substring(1, 4)
来源：http://hz.hongshengwenyu.top/gtimfginsm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtrbakjsyt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.meibo888.top/gttmtywdcu.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gthqpxbcad.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gthxjbwwuv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.andypj.xyz/gtusjpdqdr.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gtssrzjphn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtmkqyesex.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtvtbjrlkk.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtenwjbfin.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtqgtijpxn.html

Ruby: s.index("x")
来源：http://hz.jinqigfzy.top/gtfadwvfng.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtpvzlcvfg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtglbwtakr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtddczkpbr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.dashuyun.cn/gtgyivjxkk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtrwtmdeso.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gtmaegpbkv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtfnwazten.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtzisyjdja.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhaomingkeji.xyz/gtujtipnus.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.haohaochexian.top/gtmapcmtdr.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtgleezzsp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtkbfzmncc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gaohongyu789.top/gtgjrffshq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtlamrxuco.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtuxcjizyv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtqwheztlj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtgickwzjr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtsaemiqeg.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigufen.top/gtdgpmovzt.html

[E07] 按分隔符拆分
来源：http://hz.fengsongda.top/gtimqbhqru.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtrxcfuwjh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ehwqpu.com/gtzrkcslav.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangdashe.top/gtodyrscjg.html

TS:   s.split(",")
来源：http://hz.cheryme.top/gtrbfcxkue.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtkniausai.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.nanxuanxn.top/gtxbgujaih.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtlicbsbkc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nwbrower.top/gtqhfjrvym.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtvgofuewd.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtcfrthikx.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtfvuyrxut.html

JS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtopghxsbj.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtboiwyaxw.html

Java: String.join(",", items)
来源：http://hz.wangdashe.top/gtrhbbdfll.html

Go:   strings.Join(items, ",")
来源：http://hz.iojbl.cn/gtgdqpbqwy.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtkanqucuu.html

C#:   string.Join(",", items)
来源：http://hz.chenzaomai.com/gtdikhfnly.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtwnehfmcv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fengsongda.top/gtbirmdvis.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtzolobqic.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shuidangran.top/gthjapkvau.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtfgqdmmqs.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gtudohxewk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtmlikdrim.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydjk.org.cn/gtyuxsvfxo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gaohongyu789.top/gtjjnimrct.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtdtfsyqtg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtwwvunzrc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guannengcc.top/gtotekoqys.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtizyjsbsv.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtlnbvlail.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtswiuifcf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cdnleiting.top/gtlebhvocm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtqsujytpl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhixingplan.top/gthtkmkahi.html

[E11] 反转字符串
来源：http://hz.pycfn.com/gtpaitncqb.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtljvxjenl.html

PHP:  strrev($s);
来源：http://hz.ydjk.org.cn/gttrdihgvm.html

JS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtmyrlnswg.html

TS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtoykuwtyg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtweqktatn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nwbrower.top/gtfhjnviui.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtzozuuwyw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jqgfzy.top/gtqliggrdz.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtebdqeigp.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtrgvluddi.html

PHP:  substr_count($s, "a");
来源：http://hz.fengsongda.top/gtecyfxekc.html

JS:   s.split("a").length - 1
来源：http://hz.ehwqpu.com/gtqvfewkli.html

TS:   s.split("a").length - 1
来源：http://hz.birdmap.top/gtxqttxfab.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shangyingyoupin.top/gtpjtitnin.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtcbhbdodj.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtvvtunnvp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pycfn.com/gtjhddvacb.html

[E13] 逐字符遍历
来源：http://hz.cucudq.cn/gtyqemmblk.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtiwmozvfh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sysykeji.top/gtwtngbtxm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtwctvrrsz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtfidwkpze.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sufxvd.cn/gtsmempnzv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.birdmap.top/gtlmzntkeb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fzhhl.top/gtrvtanpcl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pengpengdd.cyou/gtkjjrsdmx.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangkeji.top/gtknqezukt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtfzkbxaqd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtpkwoxobk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gaohongyu789.top/gtxwvnncna.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gtwkmqtkle.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtbrxtrala.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xylfe.cn/gtjembxbuf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.snrcjt.cn/gtcmifknsh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tian-w.cn/gtsyscyooc.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenjidiqi.icu/gtzqqjxbms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.meibo888.top/gtmigtkuhw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gtltrwwygk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtwjzqvtau.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shzxlz.cn/gthgbubkgd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gthqpnuxnt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtcqauagwh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtktemxhuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinghuilouyu.cn/gtdmxndjbr.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtfjbuoeeh.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258888.top/gtdpeiazbb.html

PHP:  number_format(1234567);
来源：http://hz.c1oappe.top/gtxrxuidly.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gttuyuvbuz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtjodzfjfb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtsvbdirzu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yuanzhike.top/gthjnpdcjj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hywenlv.cn/gtjqtkxaig.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtfsddpgyf.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gtslkscpym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtnnrlwvms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtuzwomspb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gaohongyu789.top/gtxcgbtvgx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.vqdsnc.cn/gtzstctljt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yj202588.top/gtnqywjmvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cucudq.cn/gtsfgagbpx.html

Ruby: s.capitalize
来源：http://hz.jqgfzy.top/gthpluredp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuanzx.com/gtxtiympdk.html

[E18] 模板占位符替换
来源：http://hz.sufxvd.cn/gtgnmsunjh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtpwkpjkkz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gttdgrwtnr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xylfe.cn/gtyhbcuqum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtrjreczqq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenjidiqi.icu/gtzeconute.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtbieghxsv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.fengsongda.top/gtzlgwhzqf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtdcnlerba.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtlihtzaxw.html

Py:   s.splitlines()
来源：http://hz.pycfn.com/gtfdjqavas.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gaohongyu789.top/gtbbyrydir.html


<!-- 参考信息 -->