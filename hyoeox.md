代发 wailian999

[D11] 反转数组
来源：http://hz.bjfxy.top/gtnfufgjxa.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtahvzxboy.html

PHP:  array_reverse($arr);
来源：http://hz.ybcxt.top/gtbqrmngxt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtqasmsbyc.html

TS:   [...arr].reverse();
来源：http://hz.fengsongda.top/gtucaeigxe.html

Java: Collections.reverse(list);
来源：http://hz.ydzc1.top/gtvxspkxru.html

Go:   slices.Reverse(arr)
来源：http://hz.meibo888.top/gttkhjaufb.html

Ruby: arr.reverse
来源：http://hz.cheryme.top/gtbzduezvp.html

C#:   list.Reverse();
来源：http://hz.0kj1m.cn/gteanztnbf.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtbuuynagf.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtncjjxoho.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinqigufen.top/gtotcbmdhl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtszoxsmej.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtidqaifgn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtseuefzal.html

Go:   slices.Index(arr, x)
来源：http://hz.redwolf501.top/gthwmszynb.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gtvarfornd.html

C#:   list.IndexOf(x);
来源：http://hz.xingfuxueyuan.xyz/gtsvtkhxki.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtdufgnbox.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hongshengwenyu.top/gtljkvzuqh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtiycfwzbd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtubgigxzj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gthltcdxid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtsgugqjfo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtmwathxvc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenzaomai.com/gtwzladshm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhaomingkeji.xyz/gthlcothyj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgfzy.top/gtrdeycdsr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hysaishi.cn/gtgegyycgu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhongyouzk.top/gttdamyjkb.html

JS:   arr.map(x => x * 2)
来源：http://hz.ppjwa.cn/gtbznkpaef.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinghuilouyu.cn/gtjwyqptgk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gtsbujudfv.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtlytituda.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtmsnsnckl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.pengpengdd.cyou/gtkzlamann.html

[D15] 去重
来源：http://hz.xinyue.icu/gteirfnnmk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtwagpwmuo.html

PHP:  array_unique($arr);
来源：http://hz.yj202588.top/gtxrtswnyi.html

JS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtabzgkkye.html

TS:   [...new Set(arr)]
来源：http://hz.mhx1999.top/gtkvuetanp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtqwjxfblz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gtijefwilr.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gttezwmvnc.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtvsqqcmyh.html

[D16] 求和与平均值
来源：http://hz.shangyingyoupin.top/gtlhuqghti.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtfewzlqsy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtxucykfsr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yvedp.cn/gtmfineddn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ivvv.top/gtbyvprjps.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nwbrower.top/gtozewqaic.html

Go:   // 手写循环累加
来源：http://hz.cheryme.top/gtsqlcanme.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fengsongda.top/gtnwguemiq.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtkqvgvxst.html

[D17] 最大值与最小值
来源：http://hz.xuetiantiany.cn/gtbmptxipp.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtzwyenqtq.html

PHP:  max($arr);  min($arr);
来源：http://hz.yonumen.top/gtfxtznblb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ybcxt.top/gtytqryjme.html

TS:   Math.max(...arr);
来源：http://hz.sxryk.cn/gtlnytzbxu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gtlktexhdx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.pengpengdd.cyou/gtzsptuydd.html

Ruby: arr.max;  arr.min
来源：http://hz.aibaodan.cn/gtlslszvrr.html

C#:   list.Max();  list.Min()
来源：http://hz.haohaochexian.top/gtnieocchb.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gthzpukese.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuxming.cn/gttjocuwoy.html

PHP:  array_merge(...$nested);
来源：http://hz.guowangkeji.top/gtrlkqzyco.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtuphmfgwp.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gtxldegkkt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xinyue.icu/gtdwmohqcj.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtsvmsoczu.html

Ruby: nested.flatten
来源：http://hz.316326.xyz/gtbxhikgmm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtpqlagouo.html

[D19] 按字段分组
来源：http://hz.tian-w.cn/gtrefiiqxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgufenzy.top/gtoiwlkwnn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pengpengdd.cyou/gtyqswdbho.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gthzanixsq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gttvwzrpqz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hfpthk.cn/gtvdpcbdlm.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gtcdqbssfz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtmedskbkk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gttakcnhsv.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtsivmtvdn.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gtisdyvfms.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtyknizzli.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtvvfrnptl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtjpsipdod.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtotqitxoi.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gteaqqppet.html

Ruby: arr.tally
来源：http://hz.gogol.net.cn/gtjujboyyh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtchvxoyxq.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtyxoyitfx.html

Py:   x in arr
来源：http://hz.jqgufenzy.top/gtwztrorny.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gogol.net.cn/gtocorpdey.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtdmtfybjb.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtaxsudiaw.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtltfmtjug.html

Go:   slices.Contains(arr, x)
来源：http://hz.gaohongyu789.top/gtheoybdhe.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gtnjcasyge.html

C#:   list.Contains(x)
来源：http://hz.aizwys.cn/gtcajgfxfp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.c1oappe.top/gtjaguvogj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtakayxqgx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtbrhnfhxu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sufxvd.cn/gthjjbcurw.html

TS:   [...arr];
来源：http://hz.haohaochexian.top/gtodmdsknt.html

Java: new ArrayList<>(list);
来源：http://hz.c1oappe.top/gtomfhyell.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtijeairpu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yonumen.top/gtrpkpzqhn.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtsoxrzrep.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtpkdmcupw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xingfuxueyuan.xyz/gtykkrgnsd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shanyushiyangtech.top/gtimrzkwzg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258.top/gtrjujeprr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtwzjyvonk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.quarkkingdee.top/gtmgmilfia.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtcaxxozds.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtnzqtnktj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtdpnevlku.html

[D24] 字典 / Map 基本操作
来源：http://hz.yueranfly.top/gtguwsvaqz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.bjfxy.top/gtflcgpvny.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinyuanbaomall.cn/gtowdatvkx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtvafnfkgk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtjmvsiawo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sysykeji.top/gtaffmondm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daxiang520.top/gtrifpifhk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gthegoytqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xinyue.icu/gtkutzmtfd.html

[D25] Set 集合去重与交并差
来源：http://hz.fengsongda.top/gtiipspwdi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gtlrlyvruk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dianchejie.cn/gtrwqesbqo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nanxuanxn.top/gtabgykopn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sufxvd.cn/gtjfzobcvz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtdskvqrgm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtcipxlthr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtfprnixhx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daria6918.cn/gtiajzxmvg.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtyxvpyfpm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxuanxn.top/gtqvjyxudw.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtiungopso.html

JS:   arr.join(", ")
来源：http://hz.sxryk.cn/gttcifwiwa.html

TS:   arr.join(", ")
来源：http://hz.9152youxi.cn/gtwelclske.html

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtojoosoir.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ehwqpu.com/gthsvdcpfs.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtiqcyqdex.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtejgdovgr.html

================================================================================
来源：http://hz.sysykeji.top/gtblccibrz.html

E. 字符串处理
来源：http://hz.birdmap.top/gtlobxpqtz.html

================================================================================
来源：http://hz.andypj.xyz/gtjvepljpc.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtfujqufza.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hywenlv.cn/gtrbtnydze.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gzhubu.top/gtxifqfdia.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtdgemhhky.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gthovdksau.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtfxvrzzgc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhiwuduotai.top/gtothkvbva.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtgsvoqnoi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pycfn.com/gtxfldsxeo.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtiokzitwy.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtudiwnozt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hysaishi.cn/gtlmirpivi.html

JS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtoureucfb.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtcxrimqnj.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtrwrqbnas.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.9152youxi.cn/gthobqgkew.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtdfsxclpu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hfpthk.cn/gtjupbhlrk.html

[E03] 截取子串
来源：http://hz.ehwqpu.com/gtaudetbvd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgfzy.top/gtvvnepleu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jiagoushi.top/gtfyvbcjnu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtcrjtgukc.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtjrynjlnu.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtvridlsqh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtvthdnncw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.feifeiyinyue.top/gtvhxrbtim.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtozenkhxq.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangkeji.top/gtnjqavklc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtetcnvguy.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtixtggmxl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.havefunace.top/gtnviirhlm.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtrljyclay.html

Java: s.indexOf("x")
来源：http://hz.hnxiangtu.top/gtsfifpelb.html

Go:   strings.Index(s, "x")
来源：http://hz.xuetiantiany.cn/gtahadgyfx.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtymgbaaba.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gtxmglwipj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhiwuduotai.top/gtskcwuvqh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yuanzhike.top/gtvakhueid.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aizwys.cn/gtqafjlimc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtoakxgeuk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ywan-chungtsiang.top/gtieeuaaov.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtazdcmfzw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtfnuaqhjh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yanxiufei.cn/gtddgrlayp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.daria6918.cn/gtlqkievvh.html

[E06] 替换子串
来源：http://hz.xuanzx.com/gtzkajzufs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sxryk.cn/gtothubgvs.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jyoumei.cn/gtewfjalmg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtimeggtvf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtawkquije.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtusuaxjhu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenzaomai.com/gtkccdtasi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tanke756.top/gtcfryeiri.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtgpdhhoxw.html

[E07] 按分隔符拆分
来源：http://hz.yueranfly.top/gttbmbwirj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sweek.top/gtgwwvsswn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhoulong.xyz/gtuadpxwpu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtderblzqv.html

TS:   s.split(",")
来源：http://hz.hysaishi.cn/gtqkhjgpwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xylfe.cn/gtnbdqxtzq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cucudq.cn/gtbdlsprjm.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtshrrcibl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gaohongyu789.top/gtfbjthzxf.html

[E08] 数组按分隔符合并
来源：http://hz.hfpthk.cn/gtvwejlybp.html

Py:   ",".join(items)
来源：http://hz.zhijiandao.cn/gttoqdfunh.html

PHP:  implode(",", $items);
来源：http://hz.jlsjyb.cn/gtnssvesnk.html

JS:   items.join(",")
来源：http://hz.cdnleiting.top/gtdbgiaddg.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtkbynrtlw.html

Java: String.join(",", items)
来源：http://hz.shzxlz.cn/gtmmnnuges.html

Go:   strings.Join(items, ",")
来源：http://hz.ppjwa.cn/gtpqsnxmjt.html

Ruby: items.join(",")
来源：http://hz.jlsjyb.cn/gtzhgwlume.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtandwivru.html

[E09] 去除所有空白字符
来源：http://hz.nanxuanxn.top/gtpbisofep.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhixingplan.top/gtgkcpizpe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxinkj.top/gtnzukojdy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtudgqfmut.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258888.top/gtivjzztrq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sysykeji.top/gtabigisar.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cucudq.cn/gtfimiuxpm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtjfmnwmkk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtktdbeoln.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cqqwz.cn/gtnnbnidji.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daria6918.cn/gtdzqlatoi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtomzbehoc.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtljtopwht.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtxqhlejbv.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gttuttxtmi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aizwys.cn/gtihunjyom.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtifhkjhzr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ywan-chungtsiang.top/gtorhvglng.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtpqnvpugc.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtseknlens.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gtssraieoq.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtuqqkbddo.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtfgnhaetd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gtcqthkzug.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yueranfly.top/gtjorcafsy.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtnhfpstxg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtnzzipuhi.html

[E12] 统计某字符出现次数
来源：http://hz.bjfxy.top/gtrgumnnqy.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtktulvxin.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtrausaiwc.html

JS:   s.split("a").length - 1
来源：http://hz.aizwys.cn/gtshqxfuyg.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtebhdyrwr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gteyhlchfs.html

Go:   strings.Count(s, "a")
来源：http://hz.hnqzz.top/gticfcygpg.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gtqslykuqi.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hammf.cn/gtxpwalzcb.html

[E13] 逐字符遍历
来源：http://hz.hongshengwenyu.top/gtdptcuaue.html

Py:   for ch in s: print(ch)
来源：http://hz.zhongyouzk.top/gtfjlghead.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuanzhike.top/gttowszhuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gtfqaovfbu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtggyjkqxb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.snrcjt.cn/gtnmtqcyek.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gthgvysxgd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gotoacloud.top/gtrbpdzlwo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.pycfn.com/gtlgrvkauw.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigfzy.top/gtwefevhht.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hywenlv.cn/gtljnltgla.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hywenlv.cn/gtbixmtmul.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtxlonoxvp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.9152youxi.cn/gtjqvyzvqy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigufen.top/gtmagngznz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nanxinkj.top/gtmwlgeghb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sxryk.cn/gtkjhgiudq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cashguo.top/gtnbweocmc.html

[E15] HTML 转义 / 反转义
来源：http://hz.aibaodan.cn/gtxjhopzce.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtsoatfbuy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jiagoushi.top/gttjbiqnsc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ywan-chungtsiang.top/gtfspyqwqg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhixingplan.top/gtgabnbnxv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nwbrower.top/gtplcsricp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgufenzy.top/gtgtanrjod.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aibaodan.cn/gtklycgvpu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtlpbjbqxt.html

[E16] 数字千分位
来源：http://hz.9152youxi.cn/gtowxcdufz.html

Py:   f"{1234567:,}"
来源：http://hz.bjfxy.top/gtbeijyegc.html

PHP:  number_format(1234567);
来源：http://hz.hongshengwenyu.top/gtfcrewftg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtneemifiv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sxryk.cn/gtnwmwgjbo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cqqwz.cn/gteodjhokt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yanxiufei.cn/gtcrnurtik.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinghuilouyu.cn/gtiwrftwqm.html

C#:   1234567.ToString("N0")
来源：http://hz.pengpengdd.cyou/gtwgmhwsua.html

[E17] 首字母大写
来源：http://hz.zhixingplan.top/gtkffhwgvd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gteuuekcwx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhijiandao.cn/gtaaoxhtcp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtgqttlhuw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtmrqwoqxd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gaohongyu789.top/gtwnglpksm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtphivtfcg.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtrdjwaovm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtqzxyjjxn.html


<!-- 参考信息 -->