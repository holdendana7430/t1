代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomyakur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vrdbpnki.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sopqlgmu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2coaxaxhu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nmflqwus.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsdduzyc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2psfoqiuj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tmdflqdv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlylvdwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxbwxdse.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lduxmtui.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ekltfkfe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2inoposiv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2evhtvulj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cqkxiypa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rnbjqnkl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nyikhzuf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nubojmfg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ovgsbhjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2eiuvneuv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qcocrlyy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2povdnocy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mnbocbrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yopxzfnu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cveabtyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bfwjvdaf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2urxahrpn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vxatrwcp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rsffsszj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dnkoflin.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dniikkfi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wajdvrde.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fakqlwzo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pernppsh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hfgjhrzv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2gykbpbzj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zgvuofjm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtknamb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2asgyrvry.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jbuuhpgt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ymaqlgnc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2njyclzbf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fngryktk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nthnkfmv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fufuvlxs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgchjct.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ckhnicgs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aewcifao.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ovhayljd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uxmpysmt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uzgrmrph.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhyayyv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hxjhxjuf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bpbzepox.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bvieaviv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ulsbafef.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xgoubeav.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tvwnnusx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttbmxjos.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtelbfm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtjalvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fkbbgnut.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdfokxqu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tlvtgaxs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2smazelcz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jdogvftg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fziepwvd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2znsrhttb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gqsxyglq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2joepuyct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zbjfropb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2stllvxew.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvozjfp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvtoqhpf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zwvygnup.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jmkvstmv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jqekijvo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rxkgsrvd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lapqdpwf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2oxmgkbog.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xtcqchel.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2sewmweks.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vegxqdil.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ijbkxhxv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ntcualmj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xzrtyxta.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fnlobxld.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tlfjwots.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zsfisstf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yuwujlzr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tftzxbyn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rcxoemig.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xfjpqetm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2uxtixtlc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2erkiyxlf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dvxgqsix.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vfaoqsvk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivnvtkbz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cjbxogdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2snznoimk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2olrqvvid.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hzuxmojl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2olxopptc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2siaakfxv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2blymlbjx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fjcytfkk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vqjzetrs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jsvwrutu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wfrbdpii.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfbornk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2opowcsag.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tepulifh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gkvszxjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2iivxqrid.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gxbpivgh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dgdqgpst.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2glgleblf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2axhotiyc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tiqttccp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2bxtvqgdv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rfwydbhc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2czafzill.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxcttw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ubluhdqj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ggdfhxfl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2brjxcino.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tniipnmf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qrnldkaw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2izzdzccq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kcbmsvks.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2qcpiiilx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zwyplzrt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nlfoizgf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fmornukm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sitazgaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ihqikdkm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ikyserxn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pypivwlo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2poihuvfk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dcuoopdl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mesktlew.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2avnoqkic.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2brdxrprr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qtrxnzvl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2piklabfs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zjkbiwnk.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2peqfuuua.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uujygnqs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2clwibcob.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2btbpnpaw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bsnbwhat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2unhfjilv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xuaqouyo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sjadjlhc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vpvwxbrg.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbppabjg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gbzoefsy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2yuvgmayk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uosxiang.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwsjsl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmpskirs.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2hidlmnxd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejouqbni.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbiuepak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzhydii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpgpwgu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ruwtdgzl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dmztakcf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2mzrgpbqg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yfvneaue.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2upvhkbwt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmwbfld.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ggyqtfey.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wlwrmedx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sxjrhday.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2krnjwnan.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nmhnfckb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sculsrkh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2riiiumjd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2agdadtrd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2tgguwbyw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hscwomli.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2etuozecm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ywrruiwc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tknzztip.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rcnwovye.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2villoatv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqfqvjfp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2bxjumivo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vjzcdsdj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2sqpwianc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2vivjfjhx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ujbnjkjf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rmuentgc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ihvrvywt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bymscytl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rofgtxzf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wlitiuxv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2egfgrtwi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqjqcphm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eteafhxi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ywauqqkd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tykmwrba.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2osqltqov.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2fkkwtxvu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gqzntqjw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hqtibspk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wyqznduy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vjizegks.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftosdevo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rcvnimbr.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzbpkzp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bixxtkaa.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2inqikizv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocvtfrdh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2znhdjirc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gggmzdjc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vdudojqw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojvotudf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aoyuemqu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qwbhyjmc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ookjvbio.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ztrasvql.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vzwutvyu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2igdehmbn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gaflyleo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwrwsfwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aiinbtla.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tflztoih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kkuneavd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yijxkyuf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wyuqsjib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ghirnehd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2foksjkyb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wpkuabzm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qsbwnofa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aenevxmn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jxgilkys.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ccxzokam.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ryclihzi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2htgxuknu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2pyvfmjcj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lfrwlzjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pjhnnvze.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ocxfxmcv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pwpypayc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lqwabhze.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhagyufx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2btpobflo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onuzwhii.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjvxzea.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2znwonoib.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2dxihsedv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tmouqhnr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2etedzmej.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2njtngboc.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2mivrozhj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vixitspw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrmiece.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2oxlmgazh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjnejsrp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2dakbaoqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npnlaicm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lvbmskcf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pcardhnb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2srbhnuag.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jykwsmvf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wovkqbeg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2auracdfa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rlpeatni.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bzqmsukl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eiljzbeg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iehsopws.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2stbevdjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mvehoyxn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2roqbnpkm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lzvvdpmf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bkfuxnom.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bvksujet.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2dlyddmka.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gayvjauc.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ajmgsbup.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pjjpcmhn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fvzubxvs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2liroggxv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vvpefuuc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okdsjzbg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jajvdvuk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2oqeymifg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xyzhamre.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2lgezilyp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ourjvlrm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fcdzmmqu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2huofzlnp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ftjvpfwd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfxkmjgt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dvnuafuq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kvimtoiu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2agwhhusx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2fkpqeduj.html


<!-- 参考信息 -->