代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtcnowhfpo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtkqyhgknz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zdqjudy.top/gtejhmdfky.html

Go:   slices.Index(arr, x)
来源：http://hz.wangshuangyany.cn/gtrdaforkw.html

Ruby: arr.index(x)
来源：http://hz.ydzc1.top/gtmlcmffan.html

C#:   list.IndexOf(x);
来源：http://hz.hysaishi.cn/gtjxfuoubo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.snrcjt.cn/gtjppunyir.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yanxiufei.cn/gtmqrjwzfn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.daxiang520.top/gtqxpaymkh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtrrxtkvvt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtxjvkgvgj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtxilpsxjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuanzhike.top/gtigijqvby.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtfldauqvg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yangfankeji.com/gtzdvwaygs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtehofrwsw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zdqjudy.top/gtigkmmdva.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gthzykfyvn.html

JS:   arr.map(x => x * 2)
来源：http://hz.jinqigufen.top/gtlkklidbe.html

TS:   arr.map(x => x * 2)
来源：http://hz.yuxming.cn/gtymugbndq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nanxinkj.top/gtwizjonvu.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gttjzxietu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtyqhckzpk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gtzmpxnzig.html

[D15] 去重
来源：http://hz.yj20258888.top/gtyuzdguza.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gthjnrlimk.html

PHP:  array_unique($arr);
来源：http://hz.gzhubu.top/gtfxrelkni.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtjkxhegvj.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtbgagcozg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnqzz.top/gtyeyeabhh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtqcnkhyvu.html

Ruby: arr.uniq
来源：http://hz.xylfe.cn/gtozypmecu.html

C#:   list.Distinct().ToList()
来源：http://hz.tianlin.xyz/gtevgaanyt.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtyjtavqfc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258.top/gtzlltjpgq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ppjwa.cn/gtaignktim.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hfpthk.cn/gtswyqpbse.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtrcfvcofb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtaozncigz.html

Go:   // 手写循环累加
来源：http://hz.fengsongda.top/gtiarvcnom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.birdmap.top/gtkgagpsmz.html

C#:   list.Sum();  list.Average()
来源：http://hz.shzxlz.cn/gtifwwtrld.html

[D17] 最大值与最小值
来源：http://hz.jinghuilouyu.cn/gtkwfizxtq.html

Py:   max(arr);  min(arr)
来源：http://hz.vqdsnc.cn/gtulopypvz.html

PHP:  max($arr);  min($arr);
来源：http://hz.sysykeji.top/gtzinbfuja.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtruqkiyot.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtgxizpxou.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtjhvhkdnt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtamsxuwnz.html

Ruby: arr.max;  arr.min
来源：http://hz.cashguo.top/gtdqbehhxd.html

C#:   list.Max();  list.Min()
来源：http://hz.guowangkeji.top/gtxebhdpop.html

[D18] 扁平化嵌套数组
来源：http://hz.vqdsnc.cn/gtnmkzdols.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.andypj.xyz/gtwlwrlvgb.html

PHP:  array_merge(...$nested);
来源：http://hz.shuidangran.top/gtvocmcxmk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tanke756.top/gtdkrkkkzx.html

TS:   nested.flat();
来源：http://hz.ydzc1.top/gtxzqybxor.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gthqssvzfk.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtqiklseyh.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtxexqtmqt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtgkuochrw.html

[D19] 按字段分组
来源：http://hz.daria6918.cn/gtwgaiixid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhengqikj.top/gtpaggakos.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sysykeji.top/gtvybeycnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yanxiufei.cn/gtwlwczsej.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnxiangtu.top/gtmhtgozon.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pengpengdd.cyou/gtvrdxbsmm.html

Go:   // 手写 map[string][]T
来源：http://hz.jinyuanbaomall.cn/gtjwdkwpyh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigufen.top/gtmebrhlmb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gtqjvrozsm.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtxlxcwmjd.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtuxtrxbxk.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtifslflxs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtcpbuwjxs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtgronyyei.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daxiang520.top/gtzpmuepgb.html

Go:   // 手写 map[T]int
来源：http://hz.hnxiangtu.top/gtfrguicdv.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtrlqjwfyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hfpthk.cn/gtcckeryrq.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gtzgerrebt.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtxvyecizj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtetaynokd.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtwgmjtenn.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtqtbqphix.html

Java: list.contains(x)
来源：http://hz.vqdsnc.cn/gtblsqdwxt.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangshuangyany.cn/gtnwnyrbbw.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtnuekqzti.html

C#:   list.Contains(x)
来源：http://hz.yueranfly.top/gtelexrmgp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtionryzqz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtvogyfekl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hfpthk.cn/gtlpseqbzu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtsqvotvsx.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gteojudcjp.html

Java: new ArrayList<>(list);
来源：http://hz.shzxlz.cn/gtvvejjaas.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cdnleiting.top/gttpsbqjht.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gaohongyu789.top/gtjjazpwrd.html

C#:   new List<int>(list);
来源：http://hz.gotoacloud.top/gtenkplrrz.html

[D23] reduce 累积计算
来源：http://hz.dianchejie.cn/gtpjdsudlr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuanzhike.top/gtepcsekla.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtjpsjjfbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtnmqxvlrv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtxtihwcrp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtrvubjbeg.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtztkbmiyb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtqezbtfec.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtqdehcpsj.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtxsytpbwm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtqgtmlcaa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gtlpfsyhqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shzxlz.cn/gtmpjryzyj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gtvuemvrsn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gaohongyu789.top/gtnberiivt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.bjfxy.top/gtcvsuimos.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtzynkznzp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtvhbgeikc.html

[D25] Set 集合去重与交并差
来源：http://hz.ivvv.top/gttxcphgdd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtrurumjgl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtyvmmevsh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gtzxtivgwz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gthwfmexys.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.svipenyu.cn/gtwxssuuap.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.mhx1999.top/gtbtmswswu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtvzohkxtj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shuidangran.top/gtdbkjdcdf.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtclifaqjr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gteoakmqpy.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtagruxsli.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtfmmtcugl.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtxvgbtchz.html

Java: String.join(", ", list)
来源：http://hz.havefunace.top/gtuozqxzjl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtkqeyzyyx.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtlzqejjrw.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtwhoclbjo.html

================================================================================
来源：http://hz.smart0.xyz/gtvfavijoo.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtmxlheykq.html

================================================================================
来源：http://hz.haohaochexian.top/gtiaeokiag.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gtrprvcodz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hammf.cn/gtwilgzyka.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jyoumei.cn/gtlxzmrsuw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtyinmqfiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtuvufxcyf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtwjdlaosl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xylfe.cn/gtcuyiozgo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.mhx1999.top/gtvuyzvnfo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtbjqznpme.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtdjtpfqwu.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtunxxsuwh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtvdpjarco.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtazshbcpm.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtubawdpdx.html

Java: "ab".repeat(3)
来源：http://hz.havefunace.top/gtoibwuoxj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.svipenyu.cn/gtiilelsff.html

Ruby: "ab" * 3
来源：http://hz.sweek.top/gtdgehotgn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cdnleiting.top/gtsdjmimca.html

[E03] 截取子串
来源：http://hz.shanyushiyangtech.top/gtyfjdedlg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.316326.xyz/gtxmpznsou.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtvpgsoyam.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yonumen.top/gtzivujypj.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtgqptmvxv.html

Java: s.substring(1, 4)
来源：http://hz.xylfe.cn/gtrcssemqk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shangyingyoupin.top/gtkyzpjrct.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yongpay.top/gtakwoyhdd.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtjzbvocra.html

[E04] 查找子串位置
来源：http://hz.nanxinkj.top/gtfbdpsuqg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gotoacloud.top/gtcknlyyqu.html

PHP:  strpos($s, "x");
来源：http://hz.jinyuanbaomall.cn/gtavrcsahr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangtech.top/gtorrhvllh.html

TS:   s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtzxxdclbb.html

Java: s.indexOf("x")
来源：http://hz.hnqzz.top/gtogofkvvf.html

Go:   strings.Index(s, "x")
来源：http://hz.tanke756.top/gtlzqfatpl.html

Ruby: s.index("x")
来源：http://hz.hongshengwenyu.top/gtoowtqipd.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtnjplqdtl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhijiandao.cn/gtxufojwod.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtcvvqfxdp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gttctoouci.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtlpdtduds.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.smart0.xyz/gtmewjeqeo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtxuxspnar.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hammf.cn/gtafnftpzb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pycfn.com/gtfirmpwnn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtlkaiooba.html

[E06] 替换子串
来源：http://hz.316326.xyz/gtfugdqrjd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtueslwgzf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtfefsmzbb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtpssqmsiy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtrybbpzlp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtggusvzvr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.kuanghao11.cn/gtzyngmend.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gtkntnekch.html

C#:   s.Replace("a", "b")
来源：http://hz.tanke756.top/gtngitrozf.html

[E07] 按分隔符拆分
来源：http://hz.hywenlv.cn/gtkulmuchs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtulxwgetp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.bjfxy.top/gtjulkuyif.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtwuxszpkm.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gtbjpsyleo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.redwolf501.top/gtqkpvlrls.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtnyufbwwt.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxuanxn.top/gtrnwppupy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hammf.cn/gtmhinnfix.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtzpvfpoxj.html

Py:   ",".join(items)
来源：http://hz.xziqi.cn/gtaotwmkyv.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gtetdgnhvu.html

JS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtwtrwiqul.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtkfnuxvew.html

Java: String.join(",", items)
来源：http://hz.jyoumei.cn/gtuslkgntd.html

Go:   strings.Join(items, ",")
来源：http://hz.zhixingplan.top/gtwqpokdvj.html

Ruby: items.join(",")
来源：http://hz.9152youxi.cn/gtdzfckaaw.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtptxdfucj.html

[E09] 去除所有空白字符
来源：http://hz.chenlongwang.top/gtlfpjxaci.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jiagoushi.top/gtngmyinrq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgfzy.top/gtfkginbqw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtrwfwzarj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtgbktfjln.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daria6918.cn/gttthjkbno.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.316326.xyz/gtrhkchcvs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xylfe.cn/gtebmawjaw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gtcwxishyg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jiagoushi.top/gttwjddofh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.andypj.xyz/gtwjitxuba.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gtaeqwmioh.html

JS:   "7".padStart(3, "0")
来源：http://hz.wangshuangyany.cn/gtzhegljye.html

TS:   "7".padStart(3, "0")
来源：http://hz.jianghu66.top/gtjlmvhtsv.html

Java: String.format("%03d", 7)
来源：http://hz.fzhhl.top/gtvcqnavrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jlsjyb.cn/gtocbhufhe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.smart0.xyz/gttpdkmpqw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shuidangran.top/gttewwywjn.html

[E11] 反转字符串
来源：http://hz.cqqwz.cn/gtrpbnbebb.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtdlklbxkm.html

PHP:  strrev($s);
来源：http://hz.xylfe.cn/gtwbuhvbud.html

JS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtqcjtonhk.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtglnpjrue.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtmgihxbcc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gtpknmwwqo.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtroifmzmc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtftnbepcw.html

[E12] 统计某字符出现次数
来源：http://hz.jiagoushi.top/gtstnuwkxx.html

Py:   s.count("a")
来源：http://hz.dianchejie.cn/gtmzngawmu.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtfttwpujs.html

JS:   s.split("a").length - 1
来源：http://hz.gaohongyu789.top/gtmzdezxgk.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtulhzptll.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xingfuxueyuan.xyz/gtdtlidaya.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtmdthgbtn.html

Ruby: s.count("a")
来源：http://hz.ehwqpu.com/gtlshidigh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtitorrupd.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gttysrhwwt.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gtqlmudufv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnxiangtu.top/gterxytjsh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtoweuizjp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtuhvpyswc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.9152youxi.cn/gtwurubzhh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guowangkeji.top/gtijesgimt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ywan-chungtsiang.top/gthrrjvhuh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhoulong.xyz/gtrwmwbkxi.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtbfasjfsx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtcwatzzmd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.smart0.xyz/gttsejthel.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ehwqpu.com/gtumdxvffq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenjidiqi.icu/gtvstmydlb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gthubqmclb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtcbotedhr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fzhhl.top/gtawtvqvlu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtbaucbynq.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtbtsvokwb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.0kj1m.cn/gtygnfriuw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtdaaeenay.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gthtxjdrzx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtvhqwauyd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.feifeiyinyue.top/gtjzrynlge.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zdqjudy.top/gtczoyyxya.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gtcffetwjt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sufxvd.cn/gtfhqrngjw.html

[E16] 数字千分位
来源：http://hz.hfpthk.cn/gthpdyujxm.html

Py:   f"{1234567:,}"
来源：http://hz.cheryme.top/gtrdnoxkvj.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtyyezbivy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtxeafxfyw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtkwvnivpb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gtreauywso.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258888.top/gtvmeuzbmx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhongyouzk.top/gtktrsisnw.html

C#:   1234567.ToString("N0")
来源：http://hz.yueranfly.top/gtdobxanfu.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtlyrvucfu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.birdmap.top/gtkdbcyude.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aibaodan.cn/gtpbzrxjzv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtcxredexo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtpbobnwgk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tanke756.top/gtjbinwbnc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtklhfocqv.html

Ruby: s.capitalize
来源：http://hz.chenzaomai.com/gtmvoodwtu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xuetiantiany.cn/gtekbmdizf.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtivnaqmjh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.aibaodan.cn/gtgirvtaez.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gttcsgpnza.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtglieikwd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtvwnznnmo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydzc1.top/gtppatycaj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gzhubu.top/gtzdnirrmr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxinkj.top/gthbtidxnb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sufxvd.cn/gtqqfxgrqk.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtqvvnjiww.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtlnxjloml.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtjjecpuhv.html


<!-- 参考信息 -->