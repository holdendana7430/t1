代发 wailian999

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtgoquuxet.html

C#:   list.IndexOf(x);
来源：http://hz.9152youxi.cn/gtcfmbbsbo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gttxwtbaos.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtvxwjbupo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cdnleiting.top/gtdvrichdj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtrpuwbwya.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtckxuawna.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtjmqqyjkd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gtbgrekova.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aibaodan.cn/gtshnqsatf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtcwojpyer.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gtbqfaamoj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jlsjyb.cn/gthkuzpemr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sysykeji.top/gtjsjigoet.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtqnyzonai.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtcchinujw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fengsongda.top/gthgmgesbc.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gturwmxicb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.havefunace.top/gtdzowfbwl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xinyue.icu/gtodswflgg.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtyvmsmhzv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zdqjudy.top/gtcszwopja.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtwolvpujm.html

JS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtyynleqdp.html

TS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtystvgcow.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtyyjedzhu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtwxrdrmag.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gteidplraj.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtlaclqnqi.html

[D16] 求和与平均值
来源：http://hz.shuidangran.top/gthwftqimb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtrwzlemid.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtsreinkys.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtajwflqyh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtrmidbsxc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gtvwllgftb.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtasxjgsmf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gthwcdwhhx.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtkkliimuf.html

[D17] 最大值与最小值
来源：http://hz.gaohongyu789.top/gtuxqjdhiv.html

Py:   max(arr);  min(arr)
来源：http://hz.mhx1999.top/gtxspokjcc.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtahgkobsw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gttbvpfadl.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtqazzvfpc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhijiandao.cn/gtvzqwwwml.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gthwjnjdfk.html

Ruby: arr.max;  arr.min
来源：http://hz.daxiang520.top/gtdlqughtt.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtaetjtwvq.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtqbdzbesb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guowangkeji.top/gtyrohnjck.html

PHP:  array_merge(...$nested);
来源：http://hz.fengsongda.top/gtrnbnykav.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gtjtxdgmhf.html

TS:   nested.flat();
来源：http://hz.daxiang520.top/gtirmklwei.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daxiang520.top/gtdfjpnufq.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gtpmznycjp.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gtayeisgby.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gttrmaalxq.html

[D19] 按字段分组
来源：http://hz.shanyushiyangtech.top/gtylftsbst.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtcrfdzgic.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtlsbdmyjk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtzxdvgpvz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtxvqbyveg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtemjlznyd.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtunlplekx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yongpay.top/gtvnuhtnml.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtxnbzpjoy.html

[D20] 统计每个元素出现次数
来源：http://hz.vqdsnc.cn/gteesgivmk.html

Py:   Counter(arr)
来源：http://hz.ybcxt.top/gtxvpblboh.html

PHP:  array_count_values($arr);
来源：http://hz.yangfankeji.com/gtuawlswez.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtabxchpsn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yvedp.cn/gtxrgfufqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gtftmqmnll.html

Go:   // 手写 map[T]int
来源：http://hz.guannengcc.top/gtqrizxgee.html

Ruby: arr.tally
来源：http://hz.zhengqikj.top/gtnohwsamo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hammf.cn/gtliuljiod.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtzqqaerof.html

Py:   x in arr
来源：http://hz.ehwqpu.com/gthlvdxjyo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtmggsuhbs.html

JS:   arr.includes(x)
来源：http://hz.cashguo.top/gtcufupewc.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtvgjqhqjt.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gtwfcazrcj.html

Go:   slices.Contains(arr, x)
来源：http://hz.cashguo.top/gtntdxvbau.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtwoyqiawd.html

C#:   list.Contains(x)
来源：http://hz.birdmap.top/gtushwpfiw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gteuczxzwl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ppjwa.cn/gtguotofgp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sysykeji.top/gttfvhkufs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtkxwwnaob.html

TS:   [...arr];
来源：http://hz.gaohongyu789.top/gtwmxxhdpn.html

Java: new ArrayList<>(list);
来源：http://hz.zhaomingkeji.xyz/gtqjgesmws.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtnkaimkjt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.birdmap.top/gtnzyeaxkz.html

C#:   new List<int>(list);
来源：http://hz.ydzc1.top/gtmfllxdor.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtncjhuvgv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtysascodl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yangfankeji.com/gtvapshmmw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gthocwphdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gtkrvakvoh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gttsahijod.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtmfspnshh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhoulong.xyz/gtzjehxnea.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgfzy.top/gtqbcxpqdp.html

[D24] 字典 / Map 基本操作
来源：http://hz.sxryk.cn/gtxdqvsbmp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sxryk.cn/gtctificyc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtbagzmmzx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtjadyntyz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtrgpgmknd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtjyreafgw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gthfxpbvmq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ywan-chungtsiang.top/gtsphtdtok.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtidasbaue.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtynwjzyhg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gttjfcaunf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yongpay.top/gttunebchi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pengpengdd.cyou/gtirlyyojr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtmbiokccx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtmcduktoz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtsyihtxpv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daxiang520.top/gtqyfkqdlf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtjaniagzq.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtrpginxai.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtunssjckv.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtilngfqga.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtavkrjjjn.html

TS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gthsadlpct.html

Java: String.join(", ", list)
来源：http://hz.gzhubu.top/gtatzstlba.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydjk.org.cn/gtvbsuxvtn.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gtcspyyiov.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtoucimwrh.html

================================================================================
来源：http://hz.tian-w.cn/gtidpteach.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtvtceudhd.html

================================================================================
来源：http://hz.chenzaomai.com/gtuecoewof.html

[E01] 拼接字符串
来源：http://hz.sweek.top/gtrlmghndf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yueranfly.top/gtyskofyla.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gtkgdcphgn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gttandepok.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhaomingkeji.xyz/gtdwfswruy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gtodlathpa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gogol.net.cn/gtmadpeprs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtycfjgrwe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pycfn.com/gtibgubkmr.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtzfenlmua.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangtech.top/gteantvitr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.316326.xyz/gtsaoihqul.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtepeaqpxr.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtbcekejxf.html

Java: "ab".repeat(3)
来源：http://hz.xinyue.icu/gtpszqqlbu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtjpvlsxwu.html

Ruby: "ab" * 3
来源：http://hz.chenjidiqi.icu/gtkfxcouso.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gttaqlsobb.html

[E03] 截取子串
来源：http://hz.shanyushiyangkeji.top/gtirjhkoch.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtyqxefiyu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.redwolf501.top/gtrprziunl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gturpfpuqp.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtmswnaygx.html

Java: s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtsgednsnm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gtkbdoocfo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shanyushiyangtech.top/gtzrirviex.html

C#:   s.Substring(1, 3)
来源：http://hz.cashguo.top/gtdjqscpde.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtlzrdhhkz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtyhntjtbt.html

PHP:  strpos($s, "x");
来源：http://hz.zycfv.cn/gtmjqvgrij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ybcxt.top/gttetapajc.html

TS:   s.indexOf("x")
来源：http://hz.ehwqpu.com/gtqtcckmbf.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtuifttqhd.html

Go:   strings.Index(s, "x")
来源：http://hz.52xcode.cn/gtwvxmqmxz.html

Ruby: s.index("x")
来源：http://hz.zhoulong.xyz/gtgddyfzuj.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gtvqfaqyte.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtcacvabdc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtrbgontqc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtkwpizeeg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtsrdxisgn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuxming.cn/gtejtaxlzu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtarteuvqq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aizwys.cn/gtdfnpnbfg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.bjfxy.top/gthhktbxum.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtryagplaw.html

[E06] 替换子串
来源：http://hz.shuidangran.top/gtbtmtqzfc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ppjwa.cn/gtoxzvjhia.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtioefkybl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtjrqlczox.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtrsntegxu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtogbpqlvc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.316326.xyz/gtzwocesoo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ehwqpu.com/gtwyjdboru.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtfgvrfqll.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtmyfpzoib.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgufenzy.top/gtpstcvmay.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhongyouzk.top/gtpbhvtuyi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ivvv.top/gtohpjigeh.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gtgzrzshfr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gtupthachp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtvdwuinzy.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtjsboobso.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fzhhl.top/gtipqzaiwp.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtzarkcenk.html

Py:   ",".join(items)
来源：http://hz.sysykeji.top/gtrgoycedf.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtmyeujghv.html

JS:   items.join(",")
来源：http://hz.vqdsnc.cn/gtiuyuuirq.html

TS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtjqcpqdrc.html

Java: String.join(",", items)
来源：http://hz.shuidangran.top/gtcfrdzfhp.html

Go:   strings.Join(items, ",")
来源：http://hz.cashguo.top/gtibhfywyb.html

Ruby: items.join(",")
来源：http://hz.pengpengdd.cyou/gtbcgfbxfr.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtclxolnmj.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gtwnygycpr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtnupgwjbh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sufxvd.cn/gtzcitjgvo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtiueulohc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.snrcjt.cn/gtlvwoivyv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtzxommpnd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhengqikj.top/gtvyfzobkl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtjehbyihl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj202588.top/gtkrvotmmn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhiwuduotai.top/gtqctaudyp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtzzcpiens.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtwignceee.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtnoaesjrm.html

TS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gtccchgusb.html

Java: String.format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtgwhksuah.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnxiangtu.top/gtrhakbxev.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gtoysqfheu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtdrbzcefo.html

[E11] 反转字符串
来源：http://hz.daria6918.cn/gtzoeqnjjs.html

Py:   s[::-1]
来源：http://hz.pengpengdd.cyou/gtfjfiviml.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtdakcsemr.html

JS:   [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtwirzhmvb.html

TS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtcvgjuxnu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangshuangyany.cn/gtfnrygxjd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yonumen.top/gtvecwztyh.html

Ruby: s.reverse
来源：http://hz.jlsjyb.cn/gtjfgdhjur.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gthvhavakw.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtoppudgjt.html

Py:   s.count("a")
来源：http://hz.gotoacloud.top/gtanvjpqpg.html

PHP:  substr_count($s, "a");
来源：http://hz.dianchejie.cn/gtfekszlvy.html

JS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtgzuaifgq.html

TS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtedimmram.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtjaojsdoj.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxinkj.top/gtqshrrmqv.html

Ruby: s.count("a")
来源：http://hz.nanxuanxn.top/gtamoqxiyq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtxcidrkpj.html

[E13] 逐字符遍历
来源：http://hz.gaohongyu789.top/gtkwwqnokr.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gthczxanyy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgufenzy.top/gtbxmivxba.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtzomfzans.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtptntaqmo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ehwqpu.com/gtuwgykvzj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xziqi.cn/gtgtxwfnae.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hysaishi.cn/gtqxegrysr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gotoacloud.top/gtxfglydol.html

[E14] URL 编码与 Base64
来源：http://hz.9152youxi.cn/gtldwiyyud.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.dianchejie.cn/gtfwmmcnxu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ivvv.top/gtaqotnmit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtrdcnligo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtowihqaao.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ydjk.org.cn/gtfzeaoxle.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gttkuxcesa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.chenzaomai.com/gtdukdsivm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tian-w.cn/gtnxdyokfl.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtwakpzfaf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.52xcode.cn/gtoburnfiw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtsgbqsebk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sysykeji.top/gtquwlneha.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daria6918.cn/gtllyonmkd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gtixhtfjoo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtkknrlnci.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtxedyimsl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guannengcc.top/gtganfddgq.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gtojqbuigz.html

Py:   f"{1234567:,}"
来源：http://hz.zhiwuduotai.top/gtosqahiyv.html

PHP:  number_format(1234567);
来源：http://hz.sweek.top/gtakdysjkg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtbjkvjuht.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtwjkkmkyw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pycfn.com/gtskivhtxg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yangfankeji.com/gtzkjlbcgo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.316326.xyz/gtwpshjytg.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtgafydlfq.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtliwqepjl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yueranfly.top/gthiozzxis.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shangyingyoupin.top/gtiulrmuvl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gotoacloud.top/gtnlhlwihf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtfrjcfwjr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sxryk.cn/gtyierkqip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.andypj.xyz/gtszshdbsx.html

Ruby: s.capitalize
来源：http://hz.jyoumei.cn/gtulyaknkt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigufen.top/gtjuqyztfx.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtjlyrvlmf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gtwcvpfiym.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sweek.top/gtyouxqatc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shangyingyoupin.top/gtukrvhfyr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tian-w.cn/gtufvirsep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jyoumei.cn/gtheeiekxr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtcimrqxfp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtwbuskquu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ehwqpu.com/gtpycbxfuo.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtgsqgyqmu.html

Py:   s.splitlines()
来源：http://hz.bjfxy.top/gtvkzjbomt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtgccidgit.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gtkmtrjauc.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtudujfjtm.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtjjcdkodg.html

Go:   strings.Split(s, "\n")
来源：http://hz.guowangkeji.top/gtnepbnbec.html


<!-- 参考信息 -->