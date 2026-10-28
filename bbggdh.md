代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtakxrkcsd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtpwvwtxkr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.dashuyun.cn/gtdwbugjup.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gttohwcgsg.html

Ruby: arr.index(x)
来源：http://hz.jinqigfzy.top/gttibnsyot.html

C#:   list.IndexOf(x);
来源：http://hz.svipenyu.cn/gtnxfqanxm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hongshengwenyu.top/gtziduamly.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhixingplan.top/gtnbyglmph.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.mhx1999.top/gtiqqpqvwt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gttpebphei.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtyqixxkdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pengpengdd.cyou/gtukjjzrmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtepvkvfst.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gtfklfauzf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtqppauceo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ppjwa.cn/gtsohkhdcb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pengpengdd.cyou/gtkfzrwoqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gtoounifuo.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtrgvwvjhc.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtcpbsirev.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.bjfxy.top/gtmqwfcvnk.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gteizsdnlg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtgardpnni.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnqzz.top/gtiuerwbhm.html

[D15] 去重
来源：http://hz.ydzc1.top/gtqtvcyids.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gtovaxcfwh.html

PHP:  array_unique($arr);
来源：http://hz.ydjk.org.cn/gtuxsfrboe.html

JS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtvxnufpbv.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtswcvflst.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtitizihwg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.feifeiyinyue.top/gtbtjdnmep.html

Ruby: arr.uniq
来源：http://hz.zhongyouzk.top/gtztflieit.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtuzehytfa.html

[D16] 求和与平均值
来源：http://hz.cashguo.top/gtxikfqkrw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ybcxt.top/gtdzznrviy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtqoucnmuq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gtihyvkqhs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtdadezfkn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hongshengwenyu.top/gtidsykrgv.html

Go:   // 手写循环累加
来源：http://hz.birdmap.top/gtyfdocogt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gtwmtxdxxa.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gtshkysebw.html

[D17] 最大值与最小值
来源：http://hz.feifeiyinyue.top/gtgbzwwxof.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtuakgzahs.html

PHP:  max($arr);  min($arr);
来源：http://hz.snrcjt.cn/gtczfcvjel.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangdashe.top/gtlwzrjnjs.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtfhsjefnq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtnvduwess.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ehwqpu.com/gttxhcuswk.html

Ruby: arr.max;  arr.min
来源：http://hz.yvedp.cn/gtoqbtuxhn.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtttjzvgkh.html

[D18] 扁平化嵌套数组
来源：http://hz.chenjidiqi.icu/gtquuxdvhn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtrnufeslj.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtgpnetqqi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtivpckxki.html

TS:   nested.flat();
来源：http://hz.chenlongwang.top/gtzkzropbv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.52xcode.cn/gtqjgqcbhd.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtrevantnd.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtfnqsktzz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gaohongyu789.top/gtrlbqxdco.html

[D19] 按字段分组
来源：http://hz.xinyue.icu/gthhhirdcb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gtvsfrytqu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtdeogifym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yanxiufei.cn/gtyhaqmwqn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtehglayvq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.havefunace.top/gtotguxfxm.html

Go:   // 手写 map[string][]T
来源：http://hz.ydjk.org.cn/gtmoxuinwf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zycfv.cn/gtflmpuzmv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nanxuanxn.top/gtqrcmqowe.html

[D20] 统计每个元素出现次数
来源：http://hz.chenlongwang.top/gtkilpkaec.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtewagdzro.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gtqmlselxi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gturbwnany.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gttrqpyxta.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuxming.cn/gthhhvuxbo.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gtequprkmc.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtjyukdbri.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtdmecxpir.html

[D21] 判断是否包含某元素
来源：http://hz.xylfe.cn/gtgcajltqv.html

Py:   x in arr
来源：http://hz.yongpay.top/gtynjnewuh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtfvnfryxn.html

JS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gttwspzezx.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtizhzszdc.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtbpjrfwny.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtvkvzhrnj.html

Ruby: arr.include?(x)
来源：http://hz.xuetiantiany.cn/gtohisfivb.html

C#:   list.Contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtyodugxtq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtlnmcqksu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtgyfqxnxf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtvuxuudau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtysnpdwhv.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtjwbthjfp.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtxyjorquh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigufen.top/gteibjbuzl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtgrrmiumx.html

C#:   new List<int>(list);
来源：http://hz.andypj.xyz/gtsqhyfrib.html

[D23] reduce 累积计算
来源：http://hz.cucudq.cn/gtoioifqfr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtczfevggc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtqlzwituv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtyscmpnrm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dianchejie.cn/gtlxhdzwgj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shangyingyoupin.top/gtyfzrrrut.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtsboxptvb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tanke756.top/gtbsnknafc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.kuanghao11.cn/gtucwoaxkz.html

[D24] 字典 / Map 基本操作
来源：http://hz.andypj.xyz/gtkrhgdpzb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.svipenyu.cn/gtgfmclmvz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aizwys.cn/gthapjlyfl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.iojbl.cn/gtoauhnucx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nanxinkj.top/gtiwykxfvg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cashguo.top/gtqjcznwqi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtudheoskj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gthslvbvig.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cheryme.top/gtalbedkmc.html

[D25] Set 集合去重与交并差
来源：http://hz.shanyushiyangtech.top/gtqizebuog.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.kuanghao11.cn/gtmozenjzo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.snrcjt.cn/gthehugdev.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xylfe.cn/gtgaaseojb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yongpay.top/gtqbzxowtb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtznizaalt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gtqdjwuhmi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtezaqbsby.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.guannengcc.top/gtswfafzoq.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gtjyniqqvk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.bjfxy.top/gtbvpucxhg.html

PHP:  implode(", ", $arr);
来源：http://hz.zhengqikj.top/gtdcpxctve.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtbfcgadqu.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtdcyjvwvu.html

Java: String.join(", ", list)
来源：http://hz.52xcode.cn/gtbmooyrzq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhongyouzk.top/gtpuqlsrvc.html

Ruby: arr.join(", ")
来源：http://hz.ehwqpu.com/gtpzlgbgdg.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtwqmyfayk.html

================================================================================
来源：http://hz.9152youxi.cn/gtyhrgjbos.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtirdaeecl.html

================================================================================
来源：http://hz.yj202588.top/gtmnfuntrm.html

[E01] 拼接字符串
来源：http://hz.tian-w.cn/gtcqqbczhf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtczycyfpv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xuetiantiany.cn/gtyfpzhons.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gthfsvsnsc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gthfaayvup.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.quarkkingdee.top/gtjxlhxjcv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtaxzztjmw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtagmabwdr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtzmoqdrzg.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gtefqsqtjq.html

Py:   "ab" * 3
来源：http://hz.chenzaomai.com/gtyhoczvxa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gtzmczbrbk.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtoevnsclh.html

TS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtfofvneto.html

Java: "ab".repeat(3)
来源：http://hz.meibo888.top/gtsyujqbdw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtfungbrvv.html

Ruby: "ab" * 3
来源：http://hz.vqdsnc.cn/gtbajmgrht.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tanke756.top/gtuptkceip.html

[E03] 截取子串
来源：http://hz.zhijiandao.cn/gtwcuyoiwl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhengqikj.top/gthcitctvo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtehbkbzkj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtrpbnjltp.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtmmmtzgof.html

Java: s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtbyuqkkvv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtmzqndlxx.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cdnleiting.top/gtqmgtvxpq.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gtdtimunty.html

[E04] 查找子串位置
来源：http://hz.birdmap.top/gtwlkzessz.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtkvplhgri.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtvwhwbtgt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gzhubu.top/gtkxbvbeto.html

TS:   s.indexOf("x")
来源：http://hz.zhixingplan.top/gtkjzxmspz.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gtrwifntiu.html

Go:   strings.Index(s, "x")
来源：http://hz.cdnleiting.top/gtmkbedtyf.html

Ruby: s.index("x")
来源：http://hz.yj20258888.top/gtnsrswmga.html

C#:   s.IndexOf("x")
来源：http://hz.fzhhl.top/gtlgnoneuf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtzpmenzds.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yanxiufei.cn/gtyaaakbhj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtmsbvwodk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtrelkgofj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gteespqlgy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gthinshajn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ywan-chungtsiang.top/gtfqpwelky.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yongpay.top/gtatorqkck.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.316326.xyz/gtanzntuou.html

[E06] 替换子串
来源：http://hz.andypj.xyz/gtmoybptkd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gtptmtjrvl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shuidangran.top/gtufqechvd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtobkdsobo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtrmmaaqnn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtvukqkprv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuanzhike.top/gtbcvuvxzm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gtwiqpozei.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgfzy.top/gtmxkunlit.html

[E07] 按分隔符拆分
来源：http://hz.zhengqikj.top/gtxqkfcjdz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtasfvubts.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtylajmrcf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangkeji.top/gtqeunvmbu.html

TS:   s.split(",")
来源：http://hz.yangfankeji.com/gtuilzctks.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pycfn.com/gtlffxwkcj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guowangkeji.top/gtclhzpcxb.html

Ruby: s.split(",");  s.split
来源：http://hz.xinyue.icu/gtrbzetzab.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ywan-chungtsiang.top/gttgkqaxys.html

[E08] 数组按分隔符合并
来源：http://hz.shangyingyoupin.top/gthvtpstha.html

Py:   ",".join(items)
来源：http://hz.hnqzz.top/gtxaahcfbp.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtwbebawvb.html

JS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtvniimofp.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtdijselre.html

Java: String.join(",", items)
来源：http://hz.birdmap.top/gtkrepgfas.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtpdalsycu.html

Ruby: items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtdchasewq.html

C#:   string.Join(",", items)
来源：http://hz.daxiang520.top/gtougxbnyz.html

[E09] 去除所有空白字符
来源：http://hz.hammf.cn/gtlezgbmyg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hammf.cn/gtisioaowu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtdgnjiluu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtwwtypktj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtpmcrilvm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtefdrwhax.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtxurohnrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shangyingyoupin.top/gtpxchkaoo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.haohaochexian.top/gtyumruplb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dashuyun.cn/gtdngawlqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zycfv.cn/gtvfacpmuy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ybcxt.top/gtwbpbdbvq.html

JS:   "7".padStart(3, "0")
来源：http://hz.quarkkingdee.top/gthquokkso.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtpdfbccjy.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtszaoadhj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtdzkiipjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.birdmap.top/gtvqisixww.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtnogopfwr.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtnsyhtymv.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gtpzlaldgh.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gthfqeoesw.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gtezfouiwh.html

TS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtsqyriqxm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtvncrbisf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtyiaztyiy.html

Ruby: s.reverse
来源：http://hz.ydjk.org.cn/gtkcktgucm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtpmaihyit.html

[E12] 统计某字符出现次数
来源：http://hz.ydzc1.top/gtxhhhlavh.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtmtypfgrj.html

PHP:  substr_count($s, "a");
来源：http://hz.aibaodan.cn/gtnplddtzh.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtniovegpc.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtobrvgnaa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigfzy.top/gtahybwiuh.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtxzurfynf.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtqyfrbsdx.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ppjwa.cn/gtzoysneqt.html

[E13] 逐字符遍历
来源：http://hz.yj202588.top/gtyfjrumsp.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtyqoevjgl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtgsbcvxnz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtkcjdjpot.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gthptwokgz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.9152youxi.cn/gtrojdjxrm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigufen.top/gtuzaltkif.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtcktcazxh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xylfe.cn/gtcpjumtgf.html

[E14] URL 编码与 Base64
来源：http://hz.bjfxy.top/gtwtqytefd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtahiyfdxz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sxryk.cn/gtvyzysggr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtpzgrfbwj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenjidiqi.icu/gtbphlptyc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cucudq.cn/gtkwdvfslh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.mhx1999.top/gtxywjzvqm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gtcexzponi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.aizwys.cn/gtmyqbdbjb.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtcdmcytfi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.pengpengdd.cyou/gtptcsrpfc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daria6918.cn/gtwjwrwarv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gteszsiuvf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hywenlv.cn/gtyecdztkj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxinkj.top/gtwgnshdmm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gtgtlrkzjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gttmosgzzb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtzkaxqopv.html

[E16] 数字千分位
来源：http://hz.yj202588.top/gtpyjbqbok.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258.top/gtqhqorgek.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtrutumbks.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258888.top/gtwckkhikb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtmhzsvkaj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ehwqpu.com/gtwthmxyjd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtodgkhvlh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tian-w.cn/gthzaslkgm.html

C#:   1234567.ToString("N0")
来源：http://hz.tian-w.cn/gtfqpudnyn.html

[E17] 首字母大写
来源：http://hz.sufxvd.cn/gtqnmxaqcr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yuxming.cn/gtgrrihgeo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gzhubu.top/gtaghvsoxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.0kj1m.cn/gtgftmwmol.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtonttluqt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gtjmuvmoph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtolfmabys.html

Ruby: s.capitalize
来源：http://hz.cheryme.top/gtnznjudsu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jqgufenzy.top/gtafubbjmu.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtdvstkyva.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.chenjidiqi.icu/gtloisztsu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtpoibypnb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtpjwlvctu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtcgbrlfei.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj20258888.top/gtgqfgniyc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gogol.net.cn/gtltsktmbq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.redwolf501.top/gtklnbkkgq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.havefunace.top/gtlsffqkwe.html

[E19] 多行文本按行拆分
来源：http://hz.52xcode.cn/gtfzdamwtp.html

Py:   s.splitlines()
来源：http://hz.gzhubu.top/gtorkezptt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xinyue.icu/gtugphnjjv.html


<!-- 参考信息 -->