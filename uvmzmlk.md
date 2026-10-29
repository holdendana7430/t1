代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/grselgplq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gngmsfvwx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gxkyburja.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gpretmkpc.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gbwdeeblv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gtzciliuu.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gzeefsdsn.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gmcfyslqd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gswbzobgs.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gnjrzrkun.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/geqkjzafm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gjwpoivdu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvdbwgwlo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gcmcmecku.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/glrtykzmj.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gjefbwirr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdtjjddkt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gkzdneqcf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/grntldjip.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/giiywxhqa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gxvzxjybu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gtxzkieto.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gsavuzswd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gjhhmuast.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gibuluccr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghvevfjuo.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gdgxnxscw.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gpypxxzcd.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gwyuigmhy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gxcvgzjsf.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gukmorlpe.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/goumqbqxl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/ghtfhpwub.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gsrooxxvd.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkrzrrtii.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gdqzndsxs.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gppidemhd.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcfdfkazg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gkdaxwutq.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gmalmvmwk.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gzaeouwnt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/glodphhxb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gttyukdqe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gewuqlqne.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gtrfothev.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glmyinhxh.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gchhmlwtd.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/ghcahhcko.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gvxvvzvmy.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gyyzzifwd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gqrfqvuxj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gbusjyyoo.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gbxhjdpmc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gmakytebz.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gllbpvjhe.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gpshcedxz.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/ghnsqaxlp.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gmioeijww.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gpvonmxpc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gvokpacys.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gepfbxwwr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gvlwvsfbi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/ggjvlrvxy.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gcgwrkvme.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/grwtvrbcs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gfymtbwhz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/ghdddufjn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gqashkbbo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gdmmoigxl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkhhdopvp.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gomvujnnr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gadnupwdw.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gxguwdayr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gdmvteook.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gcrwaiyre.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glsgkbdgx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggadlfdfa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjhpsqbg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/glanfjkzy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/guzjvuklt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/grfcfzyev.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/grvfkhqrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/grzcaewtv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gpcyxeyyj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gsctnfama.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gavgvlniz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gvkduekga.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ggzzqnwir.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/goljssrxu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gkzwyydbd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gkaabyetk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gszrfutxg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gdqvnfbci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gypmeenxm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gowhefwtp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gdgbauqdb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gejwyaaap.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gmigswfxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/grcalzyhd.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gepwpvfru.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gpjwbkzcv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gutzzmmyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxmqgegqx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmxkjjcsh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/govyoehdt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gkrbekqkh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gfxeandgb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbspzzvco.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gazbhhfxt.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gduueyear.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gplgscede.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gelvrunit.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gocjjgnaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gbvzzpdcl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/giokhukbp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gffjqqpcv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gpexlxhuo.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gucpqzgsy.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gcnfnkseb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gixdqpjvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gmqwqpubu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/giyzsfvko.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gafajgzvr.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gdzklliwi.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqgdapeww.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghokupfyh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gpqygbnjz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/ggwbsmujc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gleuhogts.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/geywpcjqv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gpzpovlws.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/garwycyai.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/ggzxwgylh.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gbhtotuxn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gqfjnozrq.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/glbnnhkvy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/glihfzpbb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gwqgijwld.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gebdwpiaq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwwwvohld.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ggjpmiuhm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtohmtjyz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/giiupaueu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcinfnjju.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gcegcvwqr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gihnazymj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gchwlmair.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gslctoytx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gxopglmxi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/guqdiqinp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/ggokzyotx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gpqwgdelp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gixiacdeq.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gggopunja.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gmlmrynpq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/glkafqwxl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/ghgsteflv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gnyrtnewf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gdhkdpvog.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gvltehail.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/gclxwawgj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/ghfshkidq.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/ggyskmvxb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gumkevnsf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gieztvmzc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gtvweirwo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/grqkkiyvo.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/goskmxwti.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtapxsfkk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gcgzojlrn.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gvywipfbi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gweycfcjo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gfkfnpknh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gqwzkcbdm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ghatfophm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gqylmhucv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjsiruwua.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gptlajxac.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gtldytixc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gfololkno.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvujsuhql.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gwayzppsv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzqisgdte.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gsfpjaokm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gyhfpgwlu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gkzwfagvd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/grjummovj.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmygzjjyd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/gcpoewpvh.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gvtbyagur.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gyiczkpsw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gjweztwbb.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gmjsjtdfn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gyfhrgpsy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/ggkqasgxi.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gylfnxrtt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gavexsarq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gdqslhovw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/ggairavrn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gchckspta.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gaxisowam.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gsmlgdisz.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gdcqwaqmm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gjeafmtlj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gibtqnklg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gckxnlvcf.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gmmckcjqc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gmbulmcwy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/ggyfimlab.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlziisgr.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/ghbotvuqm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gkwwixmaf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gemdfudhy.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gyuebjjoc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gydqpiqpc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/glhwuhepe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gvsyrevfh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gxuqcwchs.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/grwbmenba.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gqdcnjwne.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/grmvhxkdh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gkgztydqc.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gssgwthwu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gdskzkfyo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gonojnrin.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gogjgwzgv.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/ggdltblbn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gbhihuebu.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gbtdehgwl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gehnolzoa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/giqilprmf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gzihmiwir.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/geyopsegy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/ggsmiqwcf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gnjsvhvsv.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gucucsohu.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gbkozburm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glzqpofbu.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gzvxildzm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvcdvpfrp.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/ghejhunnj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gnnvhpweo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gxizrcklc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gdqyqhufq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gsenuxzxx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/ghjyenrvf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gdkieovtd.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gihlaipuv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gammwperk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gucdodqtq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gdspnurbk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gercaforp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/ggfkhixlp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gblzuimre.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/getooumop.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gwfrbqbpo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gtoexgwpy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/guvwiwfex.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gowmukimu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gntdylchu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gxxayqpws.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gwxcjazhu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gehuaqsof.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gtgzqrica.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/grfswtrku.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fehbvm.com/Article/details/gijywokod.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gsfyeyhsz.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gtdgwqlmu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gympckwxb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glyjzdkwc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gbjrpauvg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gzdsyxytq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gjtqszysv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gvoavxaue.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gqjxtyckq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gopzgpedn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/guddctsmh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gcolngfgt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gxwelswij.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/ghrmlweoz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/geotdrorz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gnlgbxest.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gejfnkqky.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/ggepxjwbk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gtkcgrszg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gwseqpift.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gwaattnzo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gfqzlcnrs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gdikpehuc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyxqgymva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gnzejpqqi.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gwahpdkbp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gkibvqsvi.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gjvspzynd.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gjfwzxqlg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/guxomwcnr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/ggocczuxn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gdujanftu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gauyxmikh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/grjnweruc.sHtML


<!-- 参考信息 -->