代发 wailian999

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/glpbkopsp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gzqbvtqwv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gylivkqmg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gbhkpkilz.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gebjkadzw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/ggtmacwpw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/guoutehty.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdedqkuiq.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gjfzojsrk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcrloflpq.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gppscjneo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/ghpdwmfcz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/glilpytcs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gpdebcdwy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gvqpknndn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/ggsxowywa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gtexarvns.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjknadshf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gjsmypzga.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gqfscdhsm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gloouvefn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gmzgksqqg.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjpawtzlz.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gmxfqyceb.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gbdkujoqk.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gxjgndxqs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gdyrzpnqs.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gicvscnqo.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gfzogchjq.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gasympzsq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gvjnnrqet.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/giwehyank.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gbdqjttxl.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxtosndct.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gknmnfgnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gjfnjpaod.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghwdiffou.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gpysuocug.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gpybpzeno.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gbkujiiue.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/geaqsycqe.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gebrabaec.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gqjyftuor.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/grqqazsgk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gkqmftrvw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/grmnnhgaa.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gijfqyjgv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gyyynueut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gpuzcuqxz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/glkgrxzww.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjeqprjil.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gnztrekus.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/glbumufgq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghtfwkxut.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gsqmynjgd.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gmncadhhg.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gyysokkxn.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gsrysndmj.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gludnvrpr.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gktjlnkcf.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gbkypanbr.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzdpviowc.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gnpuonlaj.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/guburwvhk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gswynxirw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gcvpavlca.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtwebbjhl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbzwgxjsw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gkzoruznu.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/grfgxmqum.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gwwuizzuo.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gslolnecc.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/guzkmkvst.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gwtvodkgw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gflpejakw.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gmontcpkn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gzatgbqtb.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gvvbudqfu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gxjttuein.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gbemlbpwq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvmjacsro.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gemvmxtss.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gsxeumfyc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ggpmerzgw.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/genewooeh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/ggbniwalx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gviclhzvx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gxwbwqkma.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gyvicjhha.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gxrdzggiu.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gtdceklgv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/grnoindfm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gffdigphn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gvacnhctc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gwjocffrc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gyozqzcea.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gnlomhjup.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gruohmwit.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gekxjsdzi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gtgacaoao.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gkrfivnkj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/ghygmhqpj.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcnvvsmbc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gjudzbynf.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gmghuscre.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/guskjyasv.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gonacbftj.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gybizlqvg.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gynxxrpxs.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gxkfezpmx.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/goteczkra.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnihztt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gaytrzedq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gyeycumjf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gioxyveco.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggrtzasgb.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gwqtoaaau.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gtstfevob.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gdidtcdge.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gmyeozufj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gshybqmzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gcluwglqy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbcvqnqvy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guwkmegpk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gwcqzhkyc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gmxngxdpm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gshuppixm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gyupbejaq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gcbavzcle.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gwizpbqta.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ghudvepuu.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gupbwkgdg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/giumuzdcb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gmucospcr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/garcjwmwx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gplpkpiit.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gxqyjtitd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gywvhdicx.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtperidzj.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gnzhxgcxx.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gxgnjtamy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/ggatpjsrx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gigsxmvjp.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gmfucsydo.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gekqytaib.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/geuitcdhf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/gcmfzdcou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gthwnbayt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gwmsmbuoi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/glfnjeldr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/griumgcrs.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/grkzwjyut.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gbpojkytg.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gybbuzvon.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gjzuvhzgk.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/ghjxvhrbv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkcuornpi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gathjfzxo.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gjkzuhpbo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gwjidqtha.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gqupipgrd.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gbvryuebk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/ghpxvmdrp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gfibhtmsh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gcspgzgmn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gduzfatse.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gibsnjikh.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/ggkuelnje.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gxcnpksqn.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/grhydsaam.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gfhybjuro.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gdyutnntd.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/ghsuupqeb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gsqxbliam.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gydswdiix.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gbapxrptl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gyyznahny.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/ghogxdaii.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gkkepmeyj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gxdgrtbio.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gxgxkmfyd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gjfyxnldh.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gnshtamfx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gblhnpvtq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/grrpzvrnc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/geenspwvd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gjprlliut.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gjedrgxtm.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gewyizdlj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gbseywgml.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gakzurelt.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gdyqaoxyf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gfksjjcqh.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gcobrzhal.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gxycmgwut.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/garcizvsl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gjsssujzt.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gckiekcas.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxvjlgnba.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gfdzqeiiv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gngtzjbhf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/grairtmmy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goeddsltl.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gmdksozel.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gorrdtvni.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gbeiypcqs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gstdpabld.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gdjilzdjx.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gxapphcid.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsjussoaz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gomahsenm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gzfllpijw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzqsoiqvn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/giqcszgjr.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/guzwefyfn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gbphtvhly.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gblqvlxln.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/gybijfdvq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gopfzshfl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gcvvbewcb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gmqlexacn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gtjsijxyg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/ghjyylghk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gmonuvqjh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gjqbnczub.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/gkuwvlcrb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/goiydrbhx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gcuiynram.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gcocvirfm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gtizmboif.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gcmamtfnx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmjfgivnm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gvaqhrvwl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gigvwsmqj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/ganfmwgsm.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gifigwjgo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gnflwnktx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxdrggjkd.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gjuggvhgf.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gaakzirgr.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gqovoqddu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.zdbjq.cn/Article/details/ggotmoyqa.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gcbjjxwze.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gxbtdfcyo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpygtszmq.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gjpdiuyux.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geziivfso.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/ggcjyejya.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gkoobhkhd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghmdzehrw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gqfbwwlvg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnuzhox.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gsqwodsfu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/glhsgpfsx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gnylizwxn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/glmkvkpnz.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/geebmqqqm.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gyluxdtwe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmweqhpow.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gidqmwlms.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gzqfmjrce.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gjnoludvn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gdcgojlrk.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/ghyemsbtf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gfgsrsvad.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gmmznktlc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gedgnpifq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/guabcahrx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gvqdrvxub.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfaeyzbgf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gajxagfzd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/ghbwtvlgp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gudjtcwyo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gibmqvcwe.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gkckyztnz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzlhhzxec.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gbzrdgsei.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gpwavoebj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gopaavjeo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/giygkpgab.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gjhsjwpvp.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/guajbryzc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gkolamyxn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gmzxtdcoa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/getmtgljg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gicxeeuhz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gzqxdsasi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gqgjgztbx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtqvzvdsv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/geinfkizz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gptqtoayx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gicjaafcb.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/glvduvlje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gnvthnuuu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gvwcluayq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwsdcgcwy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbgwpkpjb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbwkeeibd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gtohdfbas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/goelzwdda.sHtML


<!-- 参考信息 -->