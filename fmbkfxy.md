代发 wailian999

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/ghwbdcxbt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gkecankgv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gutkwrtqh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gnedgfvhk.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gesuplkca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gxjiogynr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkpsgnaje.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gltklsrzx.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gygnqsmwx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjmckysrx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gjgbaxryn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/grgabknil.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gfzmenjqp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gwuxqtooo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gjjzsvcsr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gxakddsup.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gmjumuajc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gmoxpolep.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gybpyxbxm.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gpamvvxyr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/goluiicsi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gpgnenaez.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gishemikl.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/guizysedx.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/guztwrezi.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gyppyzmtj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gxuyssyco.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gmvzwwyzh.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gmzjovcit.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/giuvnrjqm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gdhzwxjyi.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/guzlnynhe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/glrkdrwsm.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gptbvtcqn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gvrjlggms.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gtrpkvxat.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gekhfvrzc.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/ggzxmkwnh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjvucvwax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnwipcpfx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gmufwpaxx.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gkiprwpqo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gpufrvnit.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gahexddzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gzanparfj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gqgauyqoe.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/ghqyrgogs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghldmfuiw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gtpknjror.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gtvukeeum.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/guakdxnei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gckffyydx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gxfuyyvhx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gwgrqfujx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gidihulav.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gyqqgfzcu.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpzfchdcg.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnectazpv.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gjxequgtc.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzoijsasj.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/grrfgrmhl.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmbpwdzgb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gvufmtzbc.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gexdqudny.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gftngbdzb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/grwnqummw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gzzpeyaen.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gkksckhza.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/goseemdrp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gyoeyftbd.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gzwkmauiv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gwpuorfnq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gfgslypqc.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gsuooeitj.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gdpzdwbjt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gilxlzcor.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gftkqovnj.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gmnmzkpcs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gxbtbjpki.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gucjofwxt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/genckhmuk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnrkodhll.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gwphdsudm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtoqgvizp.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gmbbilzcm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/glzqflzsy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/geeqtonkd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gvhujcbiw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnqloscej.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gcximfjki.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gbpmlwplt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gqleuzeip.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gocdnvpzi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gnectuyrp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gquhzbtun.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gwowahrzx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gedpndzuh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gkqbbhyle.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/grrdlomrk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/ghkztvcic.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gwzterznu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/ggujuphtt.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gltlaxhly.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gpoedmoiy.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gfyjgebcm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gsfbdcses.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gbkeptcyj.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gfezjhkbq.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gfohrztjv.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gvwxkjpah.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gnfuhbakn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gedmlrukj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqixbaofl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gufdmrylv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gievibdry.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmohhmlbq.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/glgmvksgh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gmmaavcct.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gwymuqksh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/gczakpibb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzjzxxgux.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gddhrxsyw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/guxwicbph.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gepajopvo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/ggodjzvbp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gcownswah.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gugxfiqbe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/giskniosf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gnkslvmxr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gmpyctdlj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfdgmnpzg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gydswaeaf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gnnhsrgpq.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtgbfqabp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gqkrfoasq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gqqbdxruv.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gxnjfbirm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gyynkoeuh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/geytxviea.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfyurlsip.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzlwhjlvf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/ghdzpcozt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/ghdnsnsel.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gnwfqtngh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqpagmygx.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gokipjcar.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gorokrssk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkvelspoc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gnmwefeit.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/germrpnhj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gkimxmmgv.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gdjslicgg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gqhmprhus.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/giqplzcgk.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ghflalxkk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gpsuervcc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gwqmxlmxn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gguwuulnw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gnjkewsra.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gclunxeao.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdtmpydxt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gckqqlefo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gbdtsrsam.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/ghsiwaxbz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/gticxtsng.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gcxhcvpyp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gvgghbfqg.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gihrjqqav.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gfpigfkzu.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gizkakruo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gmyhjckhr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glegwcecl.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gytaowvpr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gorxnlfpu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gwrsbchzt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gmmxfmpwq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkgmtstrk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gbtatjvhk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/geqdismvp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gppprlahv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gkhzltzfg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/geazrrzrc.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvorbxuxm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gemrbzoml.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/grzmcsosd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gqbhopdvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/ggmadbmdu.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/glreldytb.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gfxwewsjy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gcrycafro.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gpfdzuhyr.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gxwnvgekj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbclfyxif.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvxbxrgwi.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsgqnqdvb.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gouzebihx.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpemkxucg.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gewapxdxr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gxjkxtnff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gwlyprbno.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gmpcrqmpl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gofmrhyxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkwkdmkwg.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gttrdzjae.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gqsdywlnt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gtoeicopc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gqzbloutc.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gftldibgb.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gtictjzwc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gfaugalba.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gkwjvdzgm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gsmmjlbvm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxcwpxrpk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gmcfwbdru.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gsgbxaglp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gzhhngmhc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gocudjjsk.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gnilseylr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gmxzlverw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gapurcoim.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/glckerfxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gbehxunow.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gszrlgfau.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gfnplejlt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gjjgflqzg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gfevdjesc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/gagwdowvm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/guzwlvxln.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gitasqzir.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gcykrtynj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gchfccavl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gpaxdwbsq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gojrehbwp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gcwyftjxo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/ggfduylpt.sHtML

[D26] 数组转字符串
来源：http://mobile.zdbjq.cn/Article/details/gkhkqqdpl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gfwigibip.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gzdvfnuyk.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gsbehtjol.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmiiuoihe.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbbworown.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gelyyqmlm.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gxzvevmth.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gxotuhvut.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfyoxmdzj.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/grmwuckom.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grvtjkzrh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwsrhxhdl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gtzqhmksg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gsztsvtku.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gakozhjxw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gxjortuvw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gskowhwma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gurmcdzhf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gcpivlgaf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gmhlofahc.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/grclmbumh.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gycolkazs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxgskswcz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gacrzkypz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmmcuzpwt.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/glnhdqalp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtopzwv.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gehdfaffc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/goiuwxuwh.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gwsjqvncf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gmigrviqh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gyibrdnor.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/godllfuii.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/grfimlhux.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmgeyooyn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gjpkcecam.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gkjeawzsk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gyzvtzduu.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gcmljzdke.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gbjvglecw.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gkgxjplqn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gnauwmscz.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gmdsuuypw.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gpwuvyljk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gbucxldzg.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gyetexjqx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gmzrqmfiv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gjfxwcpal.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gefqxpdif.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gaeqbbydt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gbipmedhz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/ggnknjllm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gfgttrdhh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gxdjpqwcn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gkdwbciag.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/goqigkmte.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gcxrtsncu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/grisigdeh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gtksuzdbt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxsgywrrg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gumydsiii.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzltuehjj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gvbzdwlne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gtyvcjhpx.sHtML


<!-- 参考信息 -->