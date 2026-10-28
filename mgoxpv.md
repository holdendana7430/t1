代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.tanke756.top/gthfzyluiv.html

[R54] 比较两个文件
来源：http://hz.jlsjyb.cn/gtavnheqvz.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gtlcfmvmgs.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtdzcxvujv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ydjk.org.cn/gtbjvquhpp.html

[R56] 远程拷贝
来源：http://hz.yuxming.cn/gtqigqmwfd.html

scp file user@host:/path/
来源：http://hz.52xcode.cn/gtjmhrbmpa.html

[R57] 远程执行命令
来源：http://hz.9152youxi.cn/gtrpxwxsid.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtqhfnysrx.html

[R58] 下载文件
来源：http://hz.meibo888.top/gtqyxwlrsh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.0kj1m.cn/gtpemyxdeu.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtgyuzwbao.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtrsfaokoj.html

[R60] 只看 HTTP 状态码
来源：http://hz.hammf.cn/gtmmfghyzi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtrhmzoxcp.html

[R61] 磁盘占用
来源：http://hz.jlsjyb.cn/gtelrgjigs.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtkgiqkwif.html

[R62] 找最占空间的文件
来源：http://hz.jianghu66.top/gtuamiyztr.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtlnxjxhrp.html

[R63] 内存与进程
来源：http://hz.jqgfzy.top/gtatydvemx.html

free -h;  ps aux | grep nginx
来源：http://hz.hongshengwenyu.top/gtekgmtgji.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gtojuxbqmd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ywan-chungtsiang.top/gtfhwjgjuw.html

[R65] 查看端口占用
来源：http://hz.hnxiangtu.top/gtpwqinqty.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.andypj.xyz/gtrqieqfon.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtkqglejvi.html

crontab -e;  crontab -l
来源：http://hz.jlsjyb.cn/gtupunsiov.html

[R67] 生成随机十六进制串
来源：http://hz.yanxiufei.cn/gtnityctxr.html

openssl rand -hex 16
来源：http://hz.52xcode.cn/gtzymetzyi.html

[R68] 计算文件校验值
来源：http://hz.yvedp.cn/gtyzpghmuc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gthjgppndz.html

[R69] 生成随机密码
来源：http://hz.yuxming.cn/gtpbdelkjj.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtjqaxxgix.html

[R70] 时间戳与互转
来源：http://hz.yuxming.cn/gtwfoyqmmy.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gtgodqkfyu.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gtcufphbvt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtonmynuwv.html

[R72] 等待端口就绪
来源：http://hz.bjfxy.top/gteitdyppb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtyxfysgza.html

[R73] 分割大日志
来源：http://hz.ppjwa.cn/gtbvlgpxzb.html

split -l 1000 big.log part_
来源：http://hz.zycfv.cn/gtxxytqpyu.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gtpvwsryjw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtjtjlaudl.html

[R75] 导出环境变量
来源：http://hz.ydzc1.top/gttssablrq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ehwqpu.com/gtfwkpvzku.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtxenaqtki.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhongyouzk.top/gtghekcpxh.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtfgqfqnlb.html

read -rp "请输入: " ans
来源：http://hz.zhijiandao.cn/gtzqhytnay.html

[R78] 交互式菜单
来源：http://hz.chenjidiqi.icu/gttrwmnwhq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gthkgtlzgs.html

[R79] 解析命令行选项
来源：http://hz.jianghu66.top/gtgvsqehgo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtpsdkxqsb.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtkzmoactp.html

time ./run.sh
来源：http://hz.fengsongda.top/gtyfzlwvvk.html

================================================================================
来源：http://hz.zdqjudy.top/gtniamgjzc.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtnlnvxumt.html

================================================================================
来源：http://hz.ydzc1.top/gtxqzbuqnl.html

[S01] C：Hello World
来源：http://hz.ybcxt.top/gtptwlmtdk.html

#include <stdio.h>
来源：http://hz.feifeiyinyue.top/gtibnrxvbl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.iojbl.cn/gtfhouqjmk.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtluovpiur.html

int a = 10; printf("%d\n", a);
来源：http://hz.yuxming.cn/gtevdzgaps.html

[S03] C：读入整数
来源：http://hz.fzhhl.top/gtmimhqytn.html

int x; scanf("%d", &x);
来源：http://hz.sysykeji.top/gtufnfafdz.html

[S04] C：字符串复制
来源：http://hz.sufxvd.cn/gtyiowbclx.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.0kj1m.cn/gthprihfuu.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtoxtjipcd.html

strlen(s)
来源：http://hz.tanke756.top/gtpotojiaa.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtfsngmbya.html

strcmp(a, b) == 0
来源：http://hz.jinqigufen.top/gtokusicnj.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtysirilva.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gtexjsxxjr.html

[S08] C：动态内存分配与释放
来源：http://hz.redwolf501.top/gtghyzqvez.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtxfzcvsiu.html

[S09] C：结构体定义与初始化
来源：http://hz.sysykeji.top/gthmmlbnyw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jiagoushi.top/gtcvchufgk.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtrwfluqut.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtfeztujpt.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtwbuoqrbf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dianchejie.cn/gtlzgvwetk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgfzy.top/gtnzkrmawz.html

fclose(f);
来源：http://hz.fzhhl.top/gtgybcgmac.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtakbptfgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtyxnviifi.html

[S13] C：宏定义
来源：http://hz.yj202588.top/gtixjquaxy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtdojvcbjf.html

[S14] C：枚举
来源：http://hz.shzxlz.cn/gtvbygolhe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtvytyqqsv.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtbbmoxkei.html

(double) a / b
来源：http://hz.cqqwz.cn/gtqzfpigfl.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtlablglrh.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtxlgftdqi.html

[S17] C：安全拼接字符串
来源：http://hz.shangyingyoupin.top/gtrsgvbcga.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhiwuduotai.top/gtxrfiywlz.html

[S18] C：命令行参数
来源：http://hz.gotoacloud.top/gttheftmsj.html

int main(int argc, char **argv)
来源：http://hz.jiagoushi.top/gtfzxsyicp.html

[S19] C：快速排序
来源：http://hz.zhengqikj.top/gtmxqmvyas.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtujdfcxdb.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtbqchplwy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtowpklhpd.html

[S21] C：字符类别判断
来源：http://hz.hfpthk.cn/gtxkvldkjh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtcfxdnzkr.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtrkkqvfto.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xylfe.cn/gtaebvyekr.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gtiptuqjsg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtjkcnzaat.html

[S24] C：获取本地时间
来源：http://hz.jqgfzy.top/gtusodsgdd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xuanzx.com/gtqkywjyoh.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtbhriqwbk.html

memcpy(dst, src, n);
来源：http://hz.ydzc1.top/gtwrknmixr.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtsbbxluqa.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtxcvfhqsq.html

[S27] C：定义常量
来源：http://hz.zhongyouzk.top/gtqobvvttp.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtgvrzpmds.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtzvabgyty.html

static int counter = 0;
来源：http://hz.jiagoushi.top/gtnpswigtc.html

[S29] C：变参函数
来源：http://hz.aibaodan.cn/gtewsjsgug.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhijiandao.cn/gttoulnmck.html

[S30] C：头文件保护
来源：http://hz.tian-w.cn/gtpnirjvuy.html

#ifndef X_H
来源：http://hz.gaohongyu789.top/gtuugzrmhm.html

#define X_H
来源：http://hz.zhongyouzk.top/gthqqdnbtw.html

#endif
来源：http://hz.shuidangran.top/gtofacasgb.html

[S31] C++：Hello World
来源：http://hz.tanke756.top/gtonedjoiz.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtivglvqra.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.52xcode.cn/gtxybnzkxj.html

[S32] C++：字符串
来源：http://hz.xinyue.icu/gtppjjdhaf.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtkqfviocf.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gtqvnurlpx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhixingplan.top/gtjnxrrhoh.html

[S34] C++：遍历 vector
来源：http://hz.snrcjt.cn/gtnpiiaout.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jinghuilouyu.cn/gtxnnydcuh.html

[S35] C++：map
来源：http://hz.cqqwz.cn/gthfklgavg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtynqnrheh.html

[S36] C++：unordered_map
来源：http://hz.jqgufenzy.top/gtabedivrw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtbgeuqkml.html

[S37] C++：set
来源：http://hz.daria6918.cn/gthrqaypkf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtddmmuyhm.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gteusntjey.html

std::sort(v.begin(), v.end());
来源：http://hz.daria6918.cn/gtbyauojpu.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigufen.top/gtauqimowa.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtjmtmbsfl.html

[S40] C++：查找元素
来源：http://hz.xingfuxueyuan.xyz/gtrevvtkuf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.ppjwa.cn/gtqvscqxsg.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gtnnraxdlc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.vqdsnc.cn/gtyvlqsxdm.html

[S42] C++：继承与虚函数
来源：http://hz.daria6918.cn/gtdhllyxtz.html

class B : public Base { public: void f() override {} };
来源：http://hz.hysaishi.cn/gtcmfgzupf.html

[S43] C++：智能指针
来源：http://hz.xuetiantiany.cn/gtdhyihajb.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj202588.top/gtzrjhjibu.html

[S44] C++：引用传参
来源：http://hz.ydjk.org.cn/gttlcfqadp.html

void inc(int &x) { ++x; }
来源：http://hz.gaohongyu789.top/gtjytrhnli.html

[S45] C++：lambda
来源：http://hz.cashguo.top/gtaemmfvur.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.feifeiyinyue.top/gtctdifdyw.html

[S46] C++：函数模板
来源：http://hz.nanxinkj.top/gtcyukrbrn.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xinyue.icu/gtbflgtafq.html

[S47] C++：结构化绑定遍历
来源：http://hz.hongshengwenyu.top/gtwecqzoxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtjqplbbyj.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtdulffuwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ydzc1.top/gttldngela.html

while (std::getline(in, line)) { }
来源：http://hz.sweek.top/gtqyjkjvhh.html

[S49] C++：写文件
来源：http://hz.guannengcc.top/gtfgpygwzh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.wangdashe.top/gtoipoxaeg.html

[S50] C++：格式化数字
来源：http://hz.daria6918.cn/gtmflivnmr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.snrcjt.cn/gtroptcpwt.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtiwiaeuzn.html

static_cast<double>(a) / b
来源：http://hz.xuanzx.com/gtaiuesjsa.html

[S52] C++：const 与 noexcept
来源：http://hz.dashuyun.cn/gtwrisxbdt.html

int size() const noexcept { return n_; }
来源：http://hz.daria6918.cn/gtcrbidhcs.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtavdvsabu.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtkzmdpmgo.html

[S54] C++：异常处理
来源：http://hz.hnqzz.top/gtxpcpojtg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtpvfpmase.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtdsdjswmt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fzhhl.top/gtabuqmmtq.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gturcrqtah.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtvakvqlro.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtyjtpfpjs.html

constexpr int N = 10;
来源：http://hz.shzxlz.cn/gtxvruqfey.html

[S58] C++：命名空间
来源：http://hz.hysaishi.cn/gtbtccklsi.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinyuanbaomall.cn/gtfxkjpqsd.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtvdrzqwvo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pengpengdd.cyou/gtkfrqxrbr.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtnrapdeai.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gtxaagvavc.html

================================================================================
来源：http://hz.sxryk.cn/gtfkjqkgsa.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xingfuxueyuan.xyz/gtelxiigte.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzxohegry.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtfarlenww.html

println("Hello")
来源：http://hz.nanxinkj.top/gtuxaeyxuj.html

[T02] Kotlin：变量
来源：http://hz.jianghu66.top/gtyrafokux.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gtnmjhypqf.html

[T03] Kotlin：字符串模板
来源：http://hz.hnxiangtu.top/gtxmrwqham.html

"值: $b"
来源：http://hz.jyoumei.cn/gtxztwwmzs.html

[T04] Kotlin：空安全
来源：http://hz.shangyingyoupin.top/gtvjqzdnni.html

val n: String? = null;  n?.length
来源：http://hz.bjfxy.top/gtjonctmvs.html

[T05] Kotlin：when 表达式
来源：http://hz.aizwys.cn/gtcqkwqpta.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtawocehuo.html

[T06] Kotlin：集合映射
来源：http://hz.yueranfly.top/gttmwzkeav.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtvkzrqqlx.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtqoxkucss.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtmjjjikpt.html

[T08] Kotlin：数据类
来源：http://hz.zhaomingkeji.xyz/gtjkdweuuh.html

data class User(val name: String, val age: Int)
来源：http://hz.guannengcc.top/gthuwapjhp.html

[T09] Kotlin：扩展函数
来源：http://hz.gotoacloud.top/gtmajehedf.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtxjacvxio.html

[T10] Kotlin：默认参数
来源：http://hz.yonumen.top/gtcvwlhmyy.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shanyushiyangkeji.top/gtefksvrqj.html

[T11] Kotlin：协程
来源：http://hz.cucudq.cn/gteqkhqtsj.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.fengsongda.top/gtjyqfqahz.html

[T12] Kotlin：解构声明
来源：http://hz.zhaomingkeji.xyz/gtjmhyhwnt.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtipoloplc.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtrqipbzon.html

val m = mapOf("a" to 1)
来源：http://hz.haohaochexian.top/gtxxyxvoxz.html

[T14] Kotlin：循环
来源：http://hz.vqdsnc.cn/gtggpaojhx.html

for (i in 1..10) println(i)
来源：http://hz.havefunace.top/gtsjuwjhmg.html

[T15] Kotlin：接口
来源：http://hz.dashuyun.cn/gtahcdekxo.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtvvqnvzpo.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtiaofyugc.html

print("Hello")
来源：http://hz.wangshuangyany.cn/gtwvbrecmx.html

[T17] Swift：变量与常量
来源：http://hz.snrcjt.cn/gtjtwkqncq.html

var a = 1;  let b = 2
来源：http://hz.cqqwz.cn/gtnkhbnhru.html

[T18] Swift：字符串插值
来源：http://hz.zhixingplan.top/gtexqnhokr.html

"值: \(b)"
来源：http://hz.jianghu66.top/gtmljxxfaj.html

[T19] Swift：可选绑定
来源：http://hz.gogol.net.cn/gtcxrimdou.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtrlfswete.html

[T20] Swift：数组操作
来源：http://hz.vqdsnc.cn/gtokijchwe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jqgfzy.top/gtfvisvuqq.html

[T21] Swift：遍历
来源：http://hz.feifeiyinyue.top/gtuelrxaae.html

for x in a { print(x) }
来源：http://hz.xziqi.cn/gtuarmlilh.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtxvtgaowr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenlongwang.top/gtfymbixik.html

[T23] Swift：函数
来源：http://hz.aibaodan.cn/gtivjcrmhv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.zhaomingkeji.xyz/gtwaadwkzf.html

[T24] Swift：闭包
来源：http://hz.zhengqikj.top/gthpquejge.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cqqwz.cn/gtqwyjwkdc.html

[T25] Swift：结构体
来源：http://hz.c1oappe.top/gtmqatruir.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtkocyvfxk.html

[T26] Swift：类与重写
来源：http://hz.haohaochexian.top/gtfururwlb.html

class A: Base { override func f() {} }
来源：http://hz.ivvv.top/gtzuifueyn.html

[T27] Swift：错误处理
来源：http://hz.zhengqikj.top/gtyywekggn.html

do { try f() } catch { print(error) }
来源：http://hz.birdmap.top/gtadfbrryq.html

[T28] Swift：枚举
来源：http://hz.jqgufenzy.top/gtemebtgwq.html

enum Color { case red, green }
来源：http://hz.cqqwz.cn/gtissorzsr.html

[T29] Swift：guard 提前返回
来源：http://hz.ydjk.org.cn/gtilexcana.html

guard let x = opt else { return }
来源：http://hz.cucudq.cn/gtcfbgjgzy.html

[T30] Swift：协议
来源：http://hz.hfpthk.cn/gteszhlrez.html

protocol Shape { func area() -> Double }
来源：http://hz.zhaomingkeji.xyz/gtfqgisret.html

[T31] Lua：Hello World
来源：http://hz.nanxuanxn.top/gtdejwxoap.html

print("Hello")
来源：http://hz.guowangkeji.top/gthvdplplh.html

[T32] Lua：局部变量
来源：http://hz.jlsjyb.cn/gthifqzuts.html

local a = 1
来源：http://hz.cashguo.top/gtichszqbp.html

[T33] Lua：表（数组）
来源：http://hz.shzxlz.cn/gtxjtvejym.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yueranfly.top/gtqutgxfpu.html

[T34] Lua：遍历表
来源：http://hz.daria6918.cn/gtwzhxmebr.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.cheryme.top/gtaxyudfwc.html

[T35] Lua：字典表
来源：http://hz.tanke756.top/gthaipdfxn.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xinyue.icu/gtkeipqhre.html

[T36] Lua：函数
来源：http://hz.xylfe.cn/gtgrukjyfi.html

function add(a, b) return a + b end
来源：http://hz.daria6918.cn/gtfbnvtymq.html

[T37] Lua：字符串拼接
来源：http://hz.chenlongwang.top/gtetkuogfz.html

"a" .. "b"
来源：http://hz.shuidangran.top/gttllwwajo.html

[T38] Lua：条件
来源：http://hz.smart0.xyz/gtphjvjrtc.html

if x > 0 then print("正") end
来源：http://hz.guannengcc.top/gtpugxgtzg.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtodiwobfl.html

string.find(s, "%d+")
来源：http://hz.zhixingplan.top/gtvqqkqkut.html

[T40] Lua：元表
来源：http://hz.nwbrower.top/gthzuiotkh.html

setmetatable({}, { __index = base })
来源：http://hz.chenlongwang.top/gtjlndfigr.html

[T41] Perl：Hello World
来源：http://hz.pycfn.com/gtjpdtmagm.html

print "Hello\n";
来源：http://hz.gotoacloud.top/gtmrskhosw.html

[T42] Perl：变量类型
来源：http://hz.mhx1999.top/gteqgoxixn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.andypj.xyz/gtbnfylgwp.html

[T43] Perl：字符串插值
来源：http://hz.aibaodan.cn/gtzfpgeaex.html

"值: $a"
来源：http://hz.cdnleiting.top/gtatmchwsq.html

[T44] Perl：条件
来源：http://hz.daxiang520.top/gtegvdzatn.html

if ($a > 0) { print "正"; }
来源：http://hz.pycfn.com/gtudmrbmgr.html

[T45] Perl：数组遍历
来源：http://hz.xinyue.icu/gtkoetzkok.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtcczwmicx.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gtjajcarcw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinghuilouyu.cn/gtutivryep.html

[T47] Perl：正则捕获
来源：http://hz.yj20258888.top/gtsuzrseza.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.shangyingyoupin.top/gtuaqpivlu.html

[T48] Perl：正则替换
来源：http://hz.chenzaomai.com/gtsiblpude.html

$s =~ s/old/new/g;
来源：http://hz.sufxvd.cn/gtbuwgwilu.html

[T49] Perl：函数
来源：http://hz.mhx1999.top/gtpfbwrkad.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.zhaomingkeji.xyz/gtphxxofgm.html

[T50] Perl：逐行读文件
来源：http://hz.svipenyu.cn/gtoqgxmuvo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yj20258888.top/gtsvvbixgo.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.shuidangran.top/gtyylwcryl.html

[T51] Scala：Hello World
来源：http://hz.vqdsnc.cn/gtdouhljbh.html

println("Hello")
来源：http://hz.316326.xyz/gtriyylqgg.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gtrkfrldzh.html

val a = 1;  var b = 2
来源：http://hz.meibo888.top/gtqdnqesdu.html

[T53] Scala：字符串插值
来源：http://hz.vqdsnc.cn/gtcgvsuaeo.html

s"值: $b"
来源：http://hz.shzxlz.cn/gttsgbnllx.html

[T54] Scala：集合映射
来源：http://hz.smart0.xyz/gtstoilwnq.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.sysykeji.top/gtzownwvgf.html

[T55] Scala：集合过滤
来源：http://hz.daria6918.cn/gtuazgycmt.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shzxlz.cn/gterrfxjvc.html

[T56] Scala：样例类
来源：http://hz.sysykeji.top/gtlhgoqxrw.html


<!-- 参考信息 -->