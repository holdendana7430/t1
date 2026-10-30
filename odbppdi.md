代发 wailian999

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gllatwrmt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gmlywhzfl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/guuamgtgx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gqzwsskkm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gsatknnsa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gkbalfbea.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyqrmqpuf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbcofuinq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gxykrdstv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkogblaow.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/giqgcfkbx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gahnssyxg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gscvavdri.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gvtfwlqdd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gdxadvvmn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gskektquj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gfdwrypmq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gnuadkusw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gwzrikmil.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gptwrdaaz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/ganolvjmq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gkldrqgqn.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/goktnwiqk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gicdnjxxq.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/guseystxs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gzqehzmnw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gwqsgmvjg.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/grlgbmzig.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gsvabyttj.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gphlmxldu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gdipmwrdy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gpguxqxzd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gnrzfokvi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsywbleyp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gvxoigkse.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gfovtgaii.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvgnitqqj.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gfqjjrzbn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gqbijweko.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gqcrhaceu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gilbebjhp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gldfmzlsx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gsnbvwwpd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gaoklzogu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gdstpqbss.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gicvohnpl.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gxbxlwbpy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gbfaojqym.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/grrwhwcng.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gnpveywkd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gumxnhder.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/ggyivflgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghyczgwsr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvqyxkssx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gczwwgtno.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gnbpmknmh.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gzrkrxxaf.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqbgadjdw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gmafwpowp.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gtvehfjli.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gzidkmszn.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcwvhmvgs.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/ghwircwby.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gkerkexfh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gonlnhyph.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gagbkigpz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnacbstbd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/guzcwvpyf.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gwaseztuj.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gdylpujxx.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gwgsoqsbp.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gcbfbnqny.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/glaxphmiu.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gpjcbioip.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/glmtncsyn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gzmjnongc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gpfydftep.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gskutqptv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkotrdjub.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/goezfzbtp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/ggzznuyta.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gejfxqyux.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gkpgpokro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gevwxsfec.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gblmjgznc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gjxbccfdf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/glswhmzxb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gpukmtawe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghlumuwjo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpzrltjts.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gixjhjolj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gylkeiixf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gjcgjwnlk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzfdlxhoy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/graapmiwi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gekyumpkb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gyfwvplxl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gatovdjob.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gytgzxxdu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/grvhzwtsx.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gzsviuiix.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gyniyolwy.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gdgmktjkh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/ggmedzonp.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gltiqnroe.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gzdxmbulx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grnipnqce.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gtflvspgr.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gjlnbrklk.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gqfndvjfp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gmsanbhgd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gprpusreq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gnqyazxza.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gvoyuihlf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gyjcyumud.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqiqtwcig.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gondeaspk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gcddulhgt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/ggtyppolz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gtshfwwdt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.zdbjq.cn/Article/details/gogianzuk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gofwuzmgt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/glhqhbaup.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gvwyiuume.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gwtsdykeg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gfuyfrmxc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gfwdpmdkg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gzvyyxqld.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gdufubmet.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdgrfepao.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gsogmokia.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/guixanfhz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/ghkfeoapr.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gthryaewp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gljfkjjot.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gzsrpbsaq.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gosxudkus.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/geuqkdcrf.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gvacvngrj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwmzzyidv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gjcegmmvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gbalpuzau.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gfvweupsr.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/guxcvzhyq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gbkjmciak.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gtkewmlty.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gzunypaqo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpphsragx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdhfilcnr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gklmisiek.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gkmdosrlr.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gazbkhcdq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gcwzbgcpv.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gjbybjyqx.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gcxrhrxox.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gygrleoqu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfsrquvwb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gbwltkvsw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gafsznlhy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gdkaburao.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gqexozyvl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gzmvzdikq.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gofrmfpjt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gspzuferj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gvnzawnkx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gihozzbvk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gjwbnykbt.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gbqwiaspd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gcfwsrybh.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gujrvvsll.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gbssyachx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gcdalvviq.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gqyscfbed.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gjeojnwjx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gplgobbgu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gqghwbazr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gdbsexygn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/glktvzrnq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gglfrcaik.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gxvldfocu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gykvbbpdf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gyasplsae.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gkibqfnkl.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/glhhjieyc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gkgnklgmk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqilgbnks.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gcglieitx.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gdzxdhhpp.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gunqquden.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gouzbwojm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gdmwlwesi.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gnakapoup.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gjoqbpjga.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzwazbnue.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ghebqlemv.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gwpvjovrf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gklusmjpu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gxuezkhik.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gcbcuovio.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gauqtppui.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gdgbthwoc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gmftqsamj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gqpfhgkhn.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gwcfrduau.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gfxykibsz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gmarbbybk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gqmyglyyn.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gfjbhjllv.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/ganwclftc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/geuwoldck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/grstvwjqn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/grejusork.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxozfstjz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gppjjwcqu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gqaldmtvh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/geevofvms.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdwiztib.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ghhqsmstl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gziwwnaox.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gurhsvvcg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gezirqyfz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/ggjqdssfe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.zdbjq.cn/Article/details/gzsbxrmwo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gxmnnqlyy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gvirlsgiq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gvitrnrmn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gqkvcxdym.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/ghgvqckin.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gmgeefjdk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gcfsbrkxe.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gciwclgdp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/guupxexhj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/glpdvjctj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gpwfmtdcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/ggocmokst.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gqwbbpuyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gmcgjcsuf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gysafmunu.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gtjvyojnz.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gaxioutzn.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqboytall.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gizqdytkc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gwfsdktwk.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gplauawnn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghnbmoahe.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gflxbttdc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdsizdjej.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gjnvrcvwt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/glstnbdoe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gmhwevnae.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gyutusfxx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gsvlmjyab.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gnbekhoea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gjbrkllon.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gdbfixejy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcqircgzx.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ghxasergn.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gwrfhsmri.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gtcbbpskt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/giudoabia.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gjbnedrxr.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gxjpwuttu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gxemjyhyr.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gmlngaeqf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gbkhgpqty.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gtbdjvsme.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gykmaywog.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gwibqwcpl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbflbpyhx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gwdxqrfqx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gbmmvwyup.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gfkbqsboi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gkfzowtio.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/gqtmakkxo.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gkwhmknly.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gooinblia.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gwgbjoyxh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gccwjbesv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gkeaaajak.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsrgjfdqo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gqknsqecz.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gnkwsvkoi.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gvpunktsd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gnipaccmx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/ghyzldvob.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gnaqrmcuf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gruntrusf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gwvbunvvb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gwjnatrax.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gtjykdceo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/giumabkpe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gzikcxhqe.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gkvcmjymz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/grkbirmut.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gkpynmzef.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gigedmfqr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gufboppto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzxuzgnfd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfqbqxawp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsuuioxvp.sHtML


<!-- 参考信息 -->