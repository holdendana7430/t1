代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2igbesczl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wustfthk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mgevapeb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sugwjryo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwclmro.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2zlvumdrx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zsnqjptm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2pmunbpgc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pzjzgyww.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hplxxgis.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ksegigop.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jakwagtp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2uwyzvpdw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmtejqv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2chupryxx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2khigeozl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hvmamkax.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2inurcszh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xknevoyu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zrsiiulp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jtalpaqa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deaqygyl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ryajzvlj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ktgppuvo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xyfoxinw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mtincpsq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ybsuowwi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rhidylgy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nnetulzb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jiapyigu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ernjiuoa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvasennd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oiofldfr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrnjzdot.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jgtpglya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctwsqdtb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2emjtoocn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eskkkdwh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yvnbykcj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2psillzvr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lracmlji.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zsdqhobg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ezblvpcn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mvbrlndr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dosxmhdx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xllscwgi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fxikzsci.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2aydxcvei.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ojuczgoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lwoksddn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qxfyqarr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xehoaimg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2eoivrdub.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhibkuud.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hiqqxrwq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvfxlrvl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tfozjyev.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lguzdvxc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bdqhfqan.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jkbjlgco.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wmoakrjn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ruitwiqu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dxxkfvzq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2exhgjnxd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vpbwnfbq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zxvkyvfg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgtavtsr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hsbibwyf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2pixqrwdm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kkhgwpxu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hssqgprf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwiryzk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cwsvqdnq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gyfhslxf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iphdbzee.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pwfaauuj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2udagqrxf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uazdqxcy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dczeaiki.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mgrrmovt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2teptxsdx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hbhorpus.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ozzdicvk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hewschaz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tkgorxtr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzhhoelk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nncmnyxc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wxwwmfmw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2srspbcgr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znawvckk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2blaunosq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fvdvrnxh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zqfemvds.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qgxlhlsm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2epyskovn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dpwujryw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eewjvpcf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ydwjrvap.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ebblxtnt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xpykdrdr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uzrrahpq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2grdmengx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yesakaut.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qlippabg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yppfduav.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nygpdupj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqyazylc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtcevmd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmbgazq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sihtwfmt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fvebqhdj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zucaofgw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juewxukt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wtcvewpg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dupnyvgq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nqmcegss.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzaoomqq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xgxozyux.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2veqoxoqc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ynpatncj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aravhzwl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nebkaocp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lmjcruph.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2eqfinhrc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2llabrffk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pyrjbdem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gffqxqtm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cbtjsdip.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2uvitbhoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kkcfdsdd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sghducft.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rjivwitj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kqhswbou.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ypjhhyfq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lddgixcg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2xibfsqdl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2unfmqmon.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nptxwhmo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2krsgmeon.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mzpbyukf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdbcmkf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2laaryyph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cycvtgsm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cagcgxsm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tmmralfy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dhubksba.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2spgtnjnv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rewxzvtl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mqzsyzgx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xefwodgi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iptkdzee.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2yuhozqqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2fmokaowj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkraihf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsvxswc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wvlnezcf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2beovsoho.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2enaahjtl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2filuoojj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yhkcpols.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zujkrtiv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ybcubanr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mafizabf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sssccytj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2alessypg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2owyqvgpx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2whkbccnu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wagyemop.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wiapxxjm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rkvjceac.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sghhoeec.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pwzwyxgt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qgukyjsj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ajuszedq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdwgwrk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xttvtbir.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sidiqwlc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqhwjxx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2alynegkx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mnliqkno.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jlmqwawy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hjemaajm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2jqpmqzlr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2twejapnv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvlgfujz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pifutahe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcnelzqx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tuhrlsmu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ponvdjby.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ujsmrjlw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2myvafycj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bhlyfvcl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2asgfdniq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2swhsyxqw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hxzaoilm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bcomemzn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xiruvnxh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vkuswzmj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2etivkpjg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ypnfcrrc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qklfyklc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ezqgdcze.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2sgmemlig.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hmbckzfk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ytyyulds.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2uozqynaa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vnottwbt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2baejzlaj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2asrksikj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wpndrtrx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xseswfrx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2klwcygtr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vuasrnko.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lbjweepc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fkqkpacx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2uggboczl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zofkagij.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2cjfzdotp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pgrafasx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hcjfahbe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yqpkutin.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oblsyxyh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hnoledna.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dmygfgzr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ueldifss.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkrmfle.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kltnqxhx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2vgigfayg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2crijhqsg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pnpkjang.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oedlvpcc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rrnufubr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2susgggnq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mjnqiiyp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gphcxauw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vaelzrlb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bdfjnksh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fynnotsc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vpzxdzkk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2deoohmye.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tkcfuzcj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdertxh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2koziqoty.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dzawmtwv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2yxqmyroi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2anbcuodr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2odjhwndq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2dgdgcsah.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgguammx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvydghpf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2keuxhoso.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ecxqzqss.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bmhlcpjc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2znjfhnru.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hmdicomh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2aopfdbcu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ypilkcgz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ekmnvcqz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxtzdvwv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ozrmcryl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2whioania.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsljicjj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2edfohrhb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bfvngwdx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hubbhtfw.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2psmmydrm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wkltlcuq.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cjasvveo.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2alqsrnse.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2qpnvwzku.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2fvtlkinr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zgjpzfij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmhkdavx.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2qesrjvha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwdgxokv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jriliihe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2usaebzhu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsshxzax.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2heejcgzj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2uefixzdg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gnbpcoxp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrzyfbla.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ijbmazyc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkmbkhpw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gdpflkxd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2txwbgbbe.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2gzzztiof.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jwtekhfc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lmxsrvow.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uazwjzle.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2esmvvvqs.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2jwoqbdwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2kabzhmmr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2juejgdhw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xqpflpgp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2suddqztu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fwxulrpx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xuydcito.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcwnzxi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zguemzib.html


<!-- 参考信息 -->