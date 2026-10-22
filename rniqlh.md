代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwpgcctr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xamwzfcl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uonhjcoi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jnmyzaai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rqsdzwnp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ghxhwesg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2adhicakj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gvwyfrtr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2deusnshh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqqsizio.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qvloulfl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2stgfttjh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ytzdysgt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2dgpjnbgg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ygcblktd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dvirxwxt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cukemdaw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rfuzluww.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bdzhyiyg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2sebmpvxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mzchrqsk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xfcyfhoe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ieoshogu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqksdafs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jtdxrfxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swzdvyxr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tmjzkxwr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hvkdwfco.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2eqbzymrx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jtvcmbtw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zzewzbot.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ueqvpitk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uafkiesa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2addgogca.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fnxqyvvn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hcykvzqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lgzkjpeg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oymsoieo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pspdeoer.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvgdzthk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ojtqfmwz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgbaiia.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2htnillds.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctgangiy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ipbolmtx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdbhldh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bkvmflvz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cjljtrkx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fcyxgict.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hunzaeop.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mwpugnjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2goxluafn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2auwqdqkq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bhngwocb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rogbtpjo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxngbbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qydfqlbe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2youhltfk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mvmcpwit.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bypobgvb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohtyllew.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ahnztcjg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjriupym.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2toufpafz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ygkyexxi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fiwfuyry.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hpnpxrob.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2utpnspzj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tvoslwqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ksbsopvs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ssucwuco.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vnzhhkic.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxjmuxp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nldmzdmh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2owsoesjc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vpqekdsv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ywemryps.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmrjycaf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xwecsxvl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ffcgcqmc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqkezyap.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kahrumgb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2byfnuksa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fmwzspti.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hkbncvun.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ptmdjowh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aixzbges.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2incjwgjc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eqxxhgzo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jxyudbfj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2uthtptui.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xevsibyg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2rnbjoxyr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dxzpycwv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jujcbjao.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlwcoio.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvyjoxie.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvjonuqn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2grrmgedn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nygisbro.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2alqjetbv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2sxsyodgq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tecezegw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mdnghnfz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtzdnoao.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vwscyjnk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2wzjhfiwr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cczonlbx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fcohilqy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zhqnhfdi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrltwld.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ccqyfliw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sebmxybd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vncxjmvp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ftzkczmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wapxnzgm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uidweyog.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lfcwgjpe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rtaekvtg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2tqpwqmyx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ortiuajs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zyvlsrvo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wlcxzmal.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tsgjwseo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ttgpgiua.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ofeyonwg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uqciglne.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lzahryjr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2stjwficn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2avkbdoaf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hoyqdqbv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nusdiiit.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mraknqrc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2nouwiqoc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2bwcpmqoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gewzfoyj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fsnnyoia.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2orfqmjlk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ohktmcwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ryfclsee.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fvewpkwr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xctwaqub.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnmckdqa.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jfjprkhu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iiubcyrx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hdmjxdnv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwtcnpg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cjbjeorm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztbvsinf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2iatjwpqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndyfmzdz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bfecggqy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jkeongtr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2oscfyxgf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bejtbsrh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dmqpdopz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vxdtmqum.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xvvxnnre.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2xjgpzxct.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2selqbhll.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijiaxinp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zuqsakgv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ndpopvky.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyowknby.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xkhicycc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2thnuwzed.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xtmafujy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qvgbrzro.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2svhfmnlr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2spmzbusw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2hwdziowm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2timtgzbq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vmyfjryv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xqrfzanu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oalymfzi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hthhryft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2larvxpit.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vlpolewq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jupfawhh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rxcykxrg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wbrmwaar.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mesinkjq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlhjkqv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2gueeghya.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bonmluxz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2njmdsuvj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fbntxjbv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxogktje.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fudnjbod.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcvoikfm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2nhishbmc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2sfktidkj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2eakuuprd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2layeftob.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lbocnooa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lfyxqvcp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nzejcayp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iwbnilsx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxtbeqb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2korkaard.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2fqnzonnz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2smjdwhto.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ibgcfpgq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2qpubqaze.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gpebtvse.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pcaagvla.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2toezdqjp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wwmflrnm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2irtigwsi.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yreosomv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afgkwvmr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ighjlrkw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bpvcsozn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zggyfraj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rsbxdtah.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wysxhhyv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2razmbhbr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hcysmspa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2oivtkbin.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kovdntpp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yryunbvc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2efnvfpsc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2xfngftiw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2paaupies.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xkdgardq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qmqlwoeu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fybrcnas.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cmyovhdz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vhmvbiay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rboboabn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lrpaluyu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2cwojuznj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mlqlmejy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2axzyjytj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fbwebbdg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gtwioeat.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvpcacqi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fwmsajle.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwplcxe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2phxkilrl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cazywbkc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rmbourfe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vajbgttp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ukdlextf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wxalpeww.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgfjdig.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2rtevdbil.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kqibhstv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qiezibbw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bfrnedcv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdsvnsme.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ssdnavfm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ftvyegth.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rrzxkvzl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zoqbaeme.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mflzhehz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2osjnvsqc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ugkvhsij.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lqktybkz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrdwkoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqjdhzys.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2onprilef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxmdcslx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gldokxax.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2xtlusnjh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rumgeofe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lyjcwrtq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vjmbrnya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2consivur.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yqmcesxv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mhnoybnj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ptvdrqku.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsoontpc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2woakaydh.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2omemmmdr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gvoeyrlp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yvbjorvw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zpahayzz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vziglofa.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gjfoyhjc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2rjuwznnl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2yedzsxpg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2aetikmuq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vbygglcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2icdtxyak.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2uanmduan.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mzjeepfv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xhwcvesn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ivphhlma.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2pwrwwtjc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2kdmksrda.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wasirlih.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jcmustve.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vibmvoel.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rojuqwce.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bggggonr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rpgwbuej.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xdwkfmun.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhzwiex.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2sqhirzrf.html


<!-- 参考信息 -->