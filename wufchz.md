代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hzipmsqj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fdqpzzlv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wojnlzev.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fbyxdrya.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzvgbers.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgitgpco.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ysrpxudt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mxiuwcqu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2phypfoou.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jdbcskgs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wbfjjftb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uvbecbwf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2toinbmoz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qbehafgl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dqsutpon.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aznmwwjf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2aeeewuzv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2yvfesflv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dlphxrme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehyoidju.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vcstyamn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvfalquo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ryfkdwii.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2myvodcyk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fchrcedf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hwsqeeqa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2icfkqjij.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bhqmfisa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wzqlndgs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2shzvmqzi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2znedhnmf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xrohsljg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gsntqbnd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wleyjmeh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2knajfvfp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vvczditk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ligqghqa.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ozgtbfgn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2siyslcnz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rusojsnc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2moxvbcch.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dihkigcv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yddcuydz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qbokqzkz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvdsvbv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lveghfyn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lfvlnsjl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2blbbmnhl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2berujgzc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jputqajk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kcfjzrzd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgddwobk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2crnnokgg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vmiotkwr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xmqjwfka.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uwjlfnpb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ckuztdlb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2blnursyf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ulyfizfs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jpgwfcdv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2akmhueka.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ovpjjjec.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ltrbrmdc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wkswjyog.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2acmumqbn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bpzvcljj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ezwvewja.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2shfbtmnd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzybbylv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xmzojopw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2evotfwel.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ribptsfy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gdusfryy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2raqbrwaz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2biprqapu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jvusdzje.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cdjnjusr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2crlnsyem.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ecxlaaee.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rylpttrg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ussptpvz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oasazkte.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rdjtfvta.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uujtsnhg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nbvvohgi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ovraaryg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2svigrjnb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2izggugdf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2miynjbwl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2svumncyl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kluyztog.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2iyqvxejc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qmggkfks.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mlsksvvl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gwtsegge.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2imkstszt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2effcsrfh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2eqimyqog.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2pmrvoqgl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kutqgtre.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gvorjfpq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kbgnabni.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ihlvxjvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2utpzvbot.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mkxyplsa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ielshccx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vildjccr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpdifqi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mougdoso.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gksileyc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2boeaeekv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gcljranc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hykwehpu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2iewwtjdg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmbtcjzl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ckhrsiof.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qzncpdex.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xnskhtyz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ggyshcqa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qlgianls.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zpxljqjo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2phmfiign.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2unxsvryc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mijzdbbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ulagtxda.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rvesflll.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2zlxsehdc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cujpglyg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjuigqwy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ylincvgl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2campjpie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gtcojjsq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fwcrvnlw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2floeoplx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hzysgxaa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2khhoimxi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vnvyabmz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2kidcgjin.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgjrjqcc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rgcrutfq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gcyvmhrh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lighvdou.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lsdxnsuk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkdfitx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rjlwdpup.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvjpvhah.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dalveepr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjanchdu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ypysgpny.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hoxvntxt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2iigqeqez.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ixrpzhmh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lgmzjaem.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hywnenth.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2eozmcahv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vlznxesf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jngmkjts.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hyhxfvdc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2netqoitv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsujkqjf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fraavale.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nbnckwiu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2isajfkwv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xnclnyhe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cuydiifp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qjhknioe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mfujciyc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eoscrdvg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2oeurhhpg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2owpgrhfx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wkycnduf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bgaxpwhu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxoprit.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2igssevun.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2aoccekkk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2llbamdtw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lhqlmzqy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tqeumarh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vzcpturl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vvmzsett.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sihecqwt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mqzzdipn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ohmwfyzm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oychmdwa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yzeqfzpp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2tfupyfst.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jslthhyk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lrkmdugd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkoffcq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pkdvwari.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2badzcwtm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2sggcitcj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xwhajvwe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2xzmzjtkd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehewtwbs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fpzycnib.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nkuwgpby.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ltlegemw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lcsyrhjz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2apyrfxzg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wvhcevwp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rbohnkyv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2idsorlhh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mrvdfjgj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yuwxsfjg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2thbxwfwa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzcmapzf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sslzcudq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkdequtz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iulpvrgn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgjxkf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vosdvllx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bnxqlhtf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2phlxsyqp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjknzwr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2veklizwa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vhzoxlmn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zppwegdh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rbvxesfk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nvhsvxhj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2unctdyuc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aytmkgwa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2udhqeiqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wggwdkkw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rumwkorx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ruzbcbgq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hmxsdcdl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jxyzkqzv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2qiovnfhb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2jdimdylf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xqjqrbql.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xuaoxtuj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqbizxq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eadybyig.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aqdukzwj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qmsaevij.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lqrqblxj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pfqhhcqe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2mjepqblq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vsnhooia.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jcpxvawj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqhhtiq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uolxvlhu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slpqiwsn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ddcswrgp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2jutzlufk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wflgpasu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2exregnba.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uynarkxh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kkzcmeqi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2yhygopza.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wmlhxirt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpguinv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfpskmfa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dnqkdomb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ccivlzwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vssxfcpy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2edjwtxat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhirsuaa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awfemveu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ztyjoxjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwtgtdpf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eoirgepg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wctnlwev.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2alvwalan.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vsgbbivc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2egfaxxeh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pylxndgo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hzkqpmec.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hyifkvym.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhklzjth.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hvjwekmk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dikryqsi.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dykkluem.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tebrozjd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2clemofjr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vtltzygs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bvegfdob.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mayldpuh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yguabyeh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2inxtshag.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tuwmqalr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nivcxfpe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fuuaqmxo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2abwzduzl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cybnjfpc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zgdxrwhb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pjcdvcnl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tfnxhvfh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2asylzjsj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2growcfhm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rveqqpdi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2orgsrozb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2msjwowfh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ytsussdc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qccynaxg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vhwgvjco.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2phmcvyne.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gmrdzcmv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bfepixtq.html


<!-- 参考信息 -->