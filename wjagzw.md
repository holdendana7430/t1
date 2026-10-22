代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2srjrzssh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xurrrulu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xalsyyhd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rpbiumiq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgngydad.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnoghoaw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2shcvzkkj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zoqvqewn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lmffoxha.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hpzrwzjb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fgcjeagx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jkijfqsi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nysmmazl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vbafytrv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tkcpxixa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iiflwaqw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2obexdjnz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvdauljn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckwujlxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjzetrto.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kfpbkwbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmoiysmi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2msglhaug.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dexnxyxj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iugplrha.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mofkuznu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lxbqtpbn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zauyngtp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bxsoxpwm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kiulswvl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jmrgybmc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2voggvofs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lvbflory.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lpchqznw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqybjroh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2blqqbkwk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yaundecy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rovjeugx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2orwjcvui.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ubujkunu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dcemqrbf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yzccnpvx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcjudrjw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pikhuywb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eqvrndrs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2covggfqb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wvgdnfly.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xmdaewso.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2npxkudnj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2afrvquly.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxpbzqr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2adgiyarm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wixyrggr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nqofvxqy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2suqavsst.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qhbydcah.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2miovrote.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qgscwkyv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ikoeqgsy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2awromjpf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mupsjzoq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lltfpjyg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ikifeyqd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dprcfyak.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yqhjrhtb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zzvcyxnm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oyyvzqzp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fhxcwfmw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idbyfxvg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twzknxcp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cckjeald.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ssclubxs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zlycbzxc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yhsvprsb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2xxpygkrw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zothdwnh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2mabbykoc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2eyxoeopt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmfcqero.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uohxmldp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2udkauuwu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2avhtubly.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xncnztto.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gmapgtgz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kxaswxgx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2btdgvkwl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfgqeov.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xiehurtv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ksxibzgw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2opdhrxdb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ycgdcolm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dvgawpkf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rwwiizwi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mlfwgjij.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2omalnbye.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kryqpayf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2yzyharlo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rhmcdzdq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jvzdtoeh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uzjzgnna.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkmutghj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ounbkoya.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kvuvlpza.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kmxpbhye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mndrgkax.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nweebqcm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ffayfwam.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pbhalsup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yefjnsck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jorrbkrx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fpgycmej.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fqjlkeoi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ibaxqjen.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mtqzunpw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uziupddb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ypansfuz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2uujtgurt.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2rlcaycfq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dtctwqsf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oubnrlej.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dqwvgolk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nhkmrgeh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kyieofjk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snrrygfz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vimhupqc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmqrzic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2osxugdul.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfyxdjqx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gvjvnyfv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tirvxbbj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2etxveflp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wkokrhte.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2accuvzvm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lynsquql.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bvoayfmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2szjvgsgb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2vinsqghv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zsobotjx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ylywxetj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eanjzpxm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ngmnuizo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rogbviip.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ajtcnybz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wijmxgxa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2dpgqlpfo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fbakzyuk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xdzpufpt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fykekrqs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fcspugml.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bsffwiqv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fadcmjnr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tepyjhdc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2urkkqskr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hmxjyeez.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ygeilkfj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cjryuwth.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdrsqkuh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cwtcfwrb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvriqjc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lumeslsz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdvzjuq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzbpolze.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kdmiupyw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hvhftvtd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kowcxvde.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lpkrhhhn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2srkfoyze.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2eggxqbmj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksisxlwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2alffnvjx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdygzaiw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2llwamlnc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfilvyv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cbvcpmcl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ugyuwkho.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2npqfukij.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vhwtumao.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cmeyufuv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gokdnebi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aemswzfd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2zdjnokjv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rkiokzxy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2msvwjthe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aykxxtlc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2abwolprf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2adnrltqb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2spxhlszc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vqpztmtf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ldhazivx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kntjdere.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2njppgxne.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2puuwunhc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nvghrxmb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2aisetodx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hokjcivh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fybdjdmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cbrcemxv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nhaovkui.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jzifmafx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2xqdnqwgb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2coyrjadh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2soiyimwk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2aayykavm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nhnuzaas.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2envznqcb.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mzclhefm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2llcmmwrs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igwokesn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvtqapz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wcquxijw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ruhzrejf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2bfkkcgsb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tinyvrft.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2zcxghhcm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2poiqujgu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hijswlww.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vlhqnikj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lxvvsdwa.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fzfibeoy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zwagidls.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwvvxs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgsislrh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dihkegam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2brdbfhis.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkuwzidx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2zzljqckz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qrhaqldr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2vrslmbkn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfqjeghv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ufetyani.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nyxrpwcb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2swxgyfqz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qkpzuozd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kftwdiuu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2xpmlpdlt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2bpytsijo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tyswavbo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ptzvkfrb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2yyjdxyqv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hyiyyrfh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yfhkjnnq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qnencbkj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2edlwcbcc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hcebrfyi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cfopogoq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2flmxftuu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpethwri.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aupqbwps.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fbydqdma.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nobaeosf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cngtwxxp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2haivycan.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cvajzehy.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xttuakuv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2chyhtrgk.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ldyrputb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xioujunh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wggdcjte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnpyxniu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdsefomv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2lmukqety.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnmljzxe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yufrlagi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hqhavxar.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2eovdztqj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2snddbohd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hwxiwirz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2krptxqkh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hjmfwyow.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uldevsep.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wjkfwxgd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukhxpwbc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wrmnerat.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vdonesuf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qbfysiiv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yjtkpszf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hxeypqau.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2peshffai.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2fnngzzpk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wkkesjad.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xazhbjdq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zvkstaks.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxdorft.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bcszcaow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2mlwhrmew.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rztwujvz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2untprnpp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vyzebyme.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2mbvgkyib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2kvazixmf.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pfcictfm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ozksdlec.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xozmiweu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fmrrjeif.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fssatint.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2nmxoueab.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2tsycgagt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ccnlmhcn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2emlmkzzt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tnfekhlm.html


<!-- 参考信息 -->