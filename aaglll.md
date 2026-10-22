代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2orawnubr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pevarerp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pecsxnat.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vcjfnolh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2uviibiei.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jhistbqh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tdkwpiik.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bkoyfosn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2kagekfhk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewnppzdi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rbjlntgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhhyryar.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fzlezmcx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dnaoikjm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2dbldopll.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2betldsjx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2aqhxyvoj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ulzsyalg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yvyhwkao.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jrtgjzzg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2twddnoob.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbycttt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uzifwkau.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2whvrgpql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ycpbbvtf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nprkykgi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2trmnjxgn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yrafmrom.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgoaeggv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2dgtnapuy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xzandxcc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mfqwaxkx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ceigvchh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2psrkbklo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qxagnntr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ylcymrlw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kpcvpafx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dmavpjol.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2fxydhssf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2fpqoksxq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qtxbpvft.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mxiebciu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2liedpren.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypcsxyor.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zpiewvfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nclcnphc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hdkjnbzr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wyhkfzrf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qzqdonwd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oovsuuad.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2iyxndzex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2paldomni.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2syohdtri.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2heyqejqd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mhjzeopd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qetkciys.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dbvgyjdq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rdybxmbu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xvldzkxx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sijjrlqf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iarrjdea.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kdflnkkg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ztdyzkaw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2okttwofd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmshlufy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2imltsvom.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2whscbchm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2miybppch.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iuxeewmd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wrjfybow.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wkuutasd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ebdvtjcb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qkrrpcdr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mxqkpdlk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2lecdnyqm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lndtnzei.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yarrhbsi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gteunjtf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hyiahnvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhhcslq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2etcogoup.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lqcgopjh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eoditehx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hpverjrq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xuvwwepl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2avnbyegd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2grljmsod.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uqfnyrri.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mskudgyp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sxjvebns.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2prglrugw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ekvxlyhg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkoervqn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dfrhhfdj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhhkoloi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wwmtoivw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ypisikix.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nndxazoq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zfxzqocn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2zotjgelw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pnhyxcdy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xhfcudeh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vvefuopm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvlhiqyk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bevudptn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjoxiuag.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zpopmtvt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ogwhbmgb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jrbigktz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zntavpjr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2psrrlpyx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2pbmkuota.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tqwdsqwo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fsphvmmr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2rfqopitw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2tmddzhgm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sidoorju.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gygdwhhk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gaymgecc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vnzonixh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2nehklpbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hwleurwl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zfimaarq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hapblorj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjrppxbc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qlzopmqf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2uzloquoj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nwbzxxii.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2tfnyvxzn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2esnfuvxi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2voysurnu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tervlpaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2xecnhgjk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jblizkfw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kvbesmyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2wdzrvaic.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tpwquajn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2guercsnp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpcylxkk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2icgawdvo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yizfxbqk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2puqbbpjq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbdydcm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2chnupkeb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2izlwlsyk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tckpuwcy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lrffzjwn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uhlddcfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2agmjsgcp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qlrhvsjh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fsemdmxm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xarcshmn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2reaqyfch.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2yryjtban.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zwomeqbi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mozdfbds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2aluysaze.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2seqodzhz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oopqwrqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ksfbqcpo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fcbhxbcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2loyqhlsd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dreghmfj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jloqcxpt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fxgczbox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tpirvszh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2txcvtxdf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmltwfn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ivyfrwzu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kdyezxin.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2orkdhqhr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jetxwcmh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tksbfwsn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2faeilwyp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vncbklig.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2udcfsjil.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mgvzqidx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dtmdrshj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2upqcywgn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wuggnolt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nijahkyb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2hcgilodp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dpgkfxnk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ckohxfba.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2craelydf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpjvquvt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vohinzuc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dxmxoogt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aeftsepu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2lzfvdnpz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hdfdlbvm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcsjkqby.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxvbaqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rnwebddn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yplndrja.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2skdzmrwa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gemuvauv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2pvjdycpr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2euzflopo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2haqrcqpd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sqcidqyq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2xuawbyqj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgcqvvg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cckvicfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sztjejwd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ihahluow.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2znbbfrny.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gzirjrlr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vefopsvi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2aucsmgvj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2reavidax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ycbhxdif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2piahpzin.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2mhurnvwg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ervekpde.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ruvradal.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qspbamki.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nuilzcxm.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2epnfbblz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pqtewoaa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cnzghsjl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lyphwimp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2sompchil.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rkikicac.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zparwjas.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pjlqxoqo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gprwhomf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pdfwjkep.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rnxsmitz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfjyydib.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdojipo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xltazuup.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fnxcqatt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qispzjnk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ukffawfj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qzpomxgs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvoqcmy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2btrxwxtq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nddhbtzu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2nrxidrba.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wfsyfqad.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ouvrjffz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2flzeeorm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wvybettb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2uwegfgnq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkuvvin.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vsuyocci.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jgchapbd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fgljiind.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lxsvxjli.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2poobzzcr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uwyazlpq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yisxzgtw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jvqzsyqz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aghawxcd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vducxwfo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oriofaml.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jgoldwqb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ufjdhmmh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2btgtrqiq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2noyikbea.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ytvciuzh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2yyequfyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tyexryzv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lexlsube.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drodwaya.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zataakyy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uykmmkvy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wmxbgbcs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swrjbwhx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2yniqftyw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xregavww.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lviqueao.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jxhqjmuc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pqkcacnk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2grmkrmdi.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgsydkv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hkuxfixd.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jcobidqx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ilbopzvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvhmvunc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tdcdeszw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjsqxr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vyqaytlf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yaikmslg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkhscqor.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bufoycmb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mztzcpsk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2itxjtfsn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bvgihynz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2otehlyuz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ugduvrmj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wyzjexxi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rgcrbtbu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2woaibewx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2njxevjdb.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kxglnavv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lunyfigk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzptxusj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tmstdqum.html


<!-- 参考信息 -->