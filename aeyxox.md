代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtmdpqagdx.html

[R56] 远程拷贝
来源：http://hz.c1oappe.top/gtssbbirww.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtnshuqicm.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtmqoatnlu.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtxrrsomxl.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtlgiqcsil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtxtbamuio.html

[R59] 发 POST JSON
来源：http://hz.tianlin.xyz/gtasgcnmqz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gttmsfzjfp.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtbwccyboq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jlsjyb.cn/gtlvxzzzab.html

[R61] 磁盘占用
来源：http://hz.gzhubu.top/gtawugncmi.html

df -h;  du -sh *
来源：http://hz.sweek.top/gtnjjrvtis.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtmqoxjnva.html

du -ah . | sort -rh | head -10
来源：http://hz.fengsongda.top/gtexjeyrmq.html

[R63] 内存与进程
来源：http://hz.aibaodan.cn/gtdzxqpmji.html

free -h;  ps aux | grep nginx
来源：http://hz.chenlongwang.top/gtlrgqzqbi.html

[R64] 结束进程
来源：http://hz.quarkkingdee.top/gteqnabvxf.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtisyojrgj.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtsujlfeov.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtalozugyu.html

[R66] 定时任务
来源：http://hz.ppjwa.cn/gtbnchhymu.html

crontab -e;  crontab -l
来源：http://hz.jianghu66.top/gtjtwouace.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtbqpmbsiq.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtbnwxgtiw.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gttiiyjars.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.daria6918.cn/gtjcdtyjik.html

[R69] 生成随机密码
来源：http://hz.tianlin.xyz/gtejgjweay.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtzfavfnfa.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtltjqhfzf.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtisvnngtg.html

[R71] 日期格式化
来源：http://hz.meibo888.top/gtnrdzinup.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zdqjudy.top/gtbqncdxix.html

[R72] 等待端口就绪
来源：http://hz.ydzc1.top/gtujnuofpg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtxcxcjyvg.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtmsinzuyc.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtoocwroay.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gtgmivubgc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenjidiqi.icu/gtzyadhavc.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtxtyfbakj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ppjwa.cn/gtnukeusaw.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtzanimjox.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtdcuqptgh.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtulyukect.html

read -rp "请输入: " ans
来源：http://hz.xingfuxueyuan.xyz/gtxhoqnedz.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtqwopqokp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtxueximgh.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtkownkkvf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nanxinkj.top/gtcmqzefsj.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtxrdcbgpf.html

time ./run.sh
来源：http://hz.fengsongda.top/gtorkpagmv.html

================================================================================
来源：http://hz.hnqzz.top/gtnwcalydv.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gtyiyexqlc.html

================================================================================
来源：http://hz.ehwqpu.com/gtyznckasw.html

[S01] C：Hello World
来源：http://hz.aizwys.cn/gtmufszxhy.html

#include <stdio.h>
来源：http://hz.0kj1m.cn/gtqvmhogth.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nwbrower.top/gtgibbbkvs.html

[S02] C：变量与格式化输出
来源：http://hz.guannengcc.top/gtszolpoqm.html

int a = 10; printf("%d\n", a);
来源：http://hz.pengpengdd.cyou/gtcmcamwym.html

[S03] C：读入整数
来源：http://hz.havefunace.top/gtpqsuafih.html

int x; scanf("%d", &x);
来源：http://hz.wangdashe.top/gtqygajmjw.html

[S04] C：字符串复制
来源：http://hz.cheryme.top/gtudsgfjop.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.redwolf501.top/gtknsdszvo.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtyacknrts.html

strlen(s)
来源：http://hz.svipenyu.cn/gtedabhops.html

[S06] C：字符串比较
来源：http://hz.jianghu66.top/gtezubezgp.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtjjhcueit.html

[S07] C：数组遍历求和
来源：http://hz.cdnleiting.top/gtfhqisbxm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtkqerwjoh.html

[S08] C：动态内存分配与释放
来源：http://hz.pengpengdd.cyou/gtzuhllyzq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.svipenyu.cn/gtjxyxalkp.html

[S09] C：结构体定义与初始化
来源：http://hz.quarkkingdee.top/gttvtfplbp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gttfpiumyf.html

[S10] C：指针与解引用
来源：http://hz.zhongyouzk.top/gtrxjsnkdy.html

int *p = &a;  *p = 5;
来源：http://hz.yueranfly.top/gtzyqnyjtg.html

[S11] C：逐行读文件
来源：http://hz.zhengqikj.top/gtgszcljkz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj20258888.top/gtzxkbwgst.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtfghlbvdh.html

fclose(f);
来源：http://hz.hnqzz.top/gtgxiwxyat.html

[S12] C：写文件
来源：http://hz.c1oappe.top/gtiqdxtwzf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.andypj.xyz/gtgkjwcelm.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtjktnhxaq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydzc1.top/gtfnzbxrcn.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtpvcaebls.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtpzqmmjmt.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtprlprsgq.html

(double) a / b
来源：http://hz.yvedp.cn/gtkolvdntj.html

[S16] C：位操作置位
来源：http://hz.dashuyun.cn/gtjzsdzesu.html

x |= (1 << 3);
来源：http://hz.jinyuanbaomall.cn/gtzfmdmasm.html

[S17] C：安全拼接字符串
来源：http://hz.xziqi.cn/gtifsmaphc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinyuanbaomall.cn/gtgsnyxpbj.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtlnryfjso.html

int main(int argc, char **argv)
来源：http://hz.havefunace.top/gtqgrvyita.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtzcgvlvlz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtyidubsgv.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtuqpdymxn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtzambqbcv.html

[S21] C：字符类别判断
来源：http://hz.yj202588.top/gtpjjzyinp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuanzhike.top/gtlsepbiys.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gtjsxtyxbg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258.top/gtbweyzggg.html

[S23] C：随机数
来源：http://hz.xziqi.cn/gtofrdbbru.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtjuwktner.html

[S24] C：获取本地时间
来源：http://hz.pengpengdd.cyou/gtrzdgyens.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zycfv.cn/gtkdqjclyj.html

[S25] C：内存拷贝
来源：http://hz.yuxming.cn/gtcstpotxq.html

memcpy(dst, src, n);
来源：http://hz.xziqi.cn/gtzpcfruri.html

[S26] C：内存清零
来源：http://hz.xuanzx.com/gtijpfppmi.html

memset(a, 0, sizeof a);
来源：http://hz.cucudq.cn/gtjbmfwwye.html

[S27] C：定义常量
来源：http://hz.ydjk.org.cn/gtlmxlcpho.html

const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtssbypftn.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtjilvlfsv.html

static int counter = 0;
来源：http://hz.yj20258.top/gtusggorqr.html

[S29] C：变参函数
来源：http://hz.sweek.top/gtzjaqzcbm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aibaodan.cn/gtdrbebjgr.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gthdzviivb.html

#ifndef X_H
来源：http://hz.cheryme.top/gtskshgaqm.html

#define X_H
来源：http://hz.yuxming.cn/gtioiwoohe.html

#endif
来源：http://hz.fengsongda.top/gtzbjuzyvt.html

[S31] C++：Hello World
来源：http://hz.gzhubu.top/gtnurkmjcq.html

#include <iostream>
来源：http://hz.andypj.xyz/gtsnmbpjyd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258.top/gtlzatrnjq.html

[S32] C++：字符串
来源：http://hz.jinghuilouyu.cn/gtrzdricir.html

std::string s = "hi";  s += "!";
来源：http://hz.guowangkeji.top/gtpnmoeeko.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gtoivmkjtu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gtrfwedesx.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gtvgfqnmmn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhixingplan.top/gtovcsvxvy.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtcgopnugy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtswanpmze.html

[S36] C++：unordered_map
来源：http://hz.hysaishi.cn/gtfobtiomk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtywiszjyo.html

[S37] C++：set
来源：http://hz.haohaochexian.top/gtegcjxhny.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangkeji.top/gtseenwlmw.html

[S38] C++：排序
来源：http://hz.nwbrower.top/gtfabfxhnp.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtowyqwywd.html

[S39] C++：自定义比较器排序
来源：http://hz.xingfuxueyuan.xyz/gtphiscodf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.meibo888.top/gtvnonvtfp.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtpmxmakhp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.chenjidiqi.icu/gtezegfahi.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gteexigjgw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cdnleiting.top/gtbvnlshqi.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtffgkmfsq.html

class B : public Base { public: void f() override {} };
来源：http://hz.ivvv.top/gtejiepbef.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gthumbpxse.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinqigfzy.top/gtstskzitj.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtobygceuy.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtzjuajlbx.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtmftxqnik.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinghuilouyu.cn/gtazlpwxbj.html

[S46] C++：函数模板
来源：http://hz.0kj1m.cn/gtlnakbobm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.aibaodan.cn/gtxisuzmau.html

[S47] C++：结构化绑定遍历
来源：http://hz.jyoumei.cn/gtjtzczggs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtwqusudup.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtyxsmfztg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tanke756.top/gtosxadsbh.html

while (std::getline(in, line)) { }
来源：http://hz.hfpthk.cn/gtlqyycfdw.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtbeshjogy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.meibo888.top/gtzagcozky.html

[S50] C++：格式化数字
来源：http://hz.ppjwa.cn/gtfvxilbjt.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jinghuilouyu.cn/gtylfzsqlf.html

[S51] C++：显式类型转换
来源：http://hz.guowangkeji.top/gtldapicml.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtwvskosyp.html

[S52] C++：const 与 noexcept
来源：http://hz.cucudq.cn/gtqqrwgcyc.html

int size() const noexcept { return n_; }
来源：http://hz.wangshuangyany.cn/gtkxtkshal.html

[S53] C++：移动语义
来源：http://hz.xingfuxueyuan.xyz/gtbiciykvm.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtpajvypyy.html

[S54] C++：异常处理
来源：http://hz.ywan-chungtsiang.top/gthwpcbhcc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnxiangtu.top/gtkdhnzpkq.html

[S55] C++：结构化绑定
来源：http://hz.yangfankeji.com/gtuxugpklu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ivvv.top/gtzfstkxnz.html

[S56] C++：optional
来源：http://hz.hongshengwenyu.top/gtoooifkyn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenzaomai.com/gtbjubuutd.html

[S57] C++：编译期常量
来源：http://hz.fzhhl.top/gtbwqsjidl.html

constexpr int N = 10;
来源：http://hz.52xcode.cn/gtoyogzjrh.html

[S58] C++：命名空间
来源：http://hz.jinqigufen.top/gtznjtikmr.html

namespace ns { int f() { return 1; } }
来源：http://hz.meibo888.top/gttpnxklye.html

[S59] C++：静态断言
来源：http://hz.sweek.top/gtwffdanzz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ydzc1.top/gtkvvvobtw.html

[S60] C++：遍历并删除元素
来源：http://hz.yuanzhike.top/gtminfgrto.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cheryme.top/gtowhosgqd.html

================================================================================
来源：http://hz.zhixingplan.top/gtlkhtljrv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.cqqwz.cn/gtjtgxuyzf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtylehdigr.html

[T01] Kotlin：Hello World
来源：http://hz.jinqigfzy.top/gtvyphoehq.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtgkemjjaf.html

[T02] Kotlin：变量
来源：http://hz.svipenyu.cn/gtpqrcalwf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.andypj.xyz/gtenurkmpc.html

[T03] Kotlin：字符串模板
来源：http://hz.yvedp.cn/gtdmbraegc.html

"值: $b"
来源：http://hz.andypj.xyz/gtymuyfxcf.html

[T04] Kotlin：空安全
来源：http://hz.ivvv.top/gtmqafusgp.html

val n: String? = null;  n?.length
来源：http://hz.jinyuanbaomall.cn/gtgkzudjvz.html

[T05] Kotlin：when 表达式
来源：http://hz.haohaochexian.top/gtcvwaxzce.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gtxcfytzfa.html

[T06] Kotlin：集合映射
来源：http://hz.jqgufenzy.top/gtqzhhtanw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xinyue.icu/gtyvcycemq.html

[T07] Kotlin：集合过滤
来源：http://hz.yangfankeji.com/gtbjzdbomq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.feifeiyinyue.top/gtmpsjissn.html

[T08] Kotlin：数据类
来源：http://hz.chenlongwang.top/gtcfzwlpir.html

data class User(val name: String, val age: Int)
来源：http://hz.yongpay.top/gtswtgdlqx.html

[T09] Kotlin：扩展函数
来源：http://hz.hnqzz.top/gtzdqpqmrp.html

fun String.exclaim() = this + "!"
来源：http://hz.cheryme.top/gtlpvduipi.html

[T10] Kotlin：默认参数
来源：http://hz.yj202588.top/gtpaciluvs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.svipenyu.cn/gthfluwcwk.html

[T11] Kotlin：协程
来源：http://hz.zdqjudy.top/gtdwpgtqdz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xuetiantiany.cn/gtjyysyjic.html

[T12] Kotlin：解构声明
来源：http://hz.svipenyu.cn/gtbeblfuae.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtzrfzejln.html

[T13] Kotlin：只读 Map
来源：http://hz.chenjidiqi.icu/gtcjlvvtmf.html

val m = mapOf("a" to 1)
来源：http://hz.xingfuxueyuan.xyz/gtknrwyjjl.html

[T14] Kotlin：循环
来源：http://hz.xinyue.icu/gtszjceqjr.html

for (i in 1..10) println(i)
来源：http://hz.sweek.top/gtvrnlqcli.html

[T15] Kotlin：接口
来源：http://hz.hnqzz.top/gtryqxstts.html

interface Shape { fun area(): Double }
来源：http://hz.hnqzz.top/gtjcdlmtqg.html

[T16] Swift：Hello World
来源：http://hz.wangshuangyany.cn/gtpavvyzhl.html

print("Hello")
来源：http://hz.jinqigufen.top/gtpgzggovp.html

[T17] Swift：变量与常量
来源：http://hz.hfpthk.cn/gtoktifrqx.html

var a = 1;  let b = 2
来源：http://hz.gaohongyu789.top/gtpxyrciii.html

[T18] Swift：字符串插值
来源：http://hz.yvedp.cn/gtvkpnujrr.html

"值: \(b)"
来源：http://hz.yj202588.top/gtbujgsegl.html

[T19] Swift：可选绑定
来源：http://hz.sweek.top/gtuzyxfawc.html

if let n = opt { print(n) }
来源：http://hz.guannengcc.top/gtbarxoguc.html

[T20] Swift：数组操作
来源：http://hz.svipenyu.cn/gtxchadotd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jlsjyb.cn/gtdvqmbgez.html

[T21] Swift：遍历
来源：http://hz.9152youxi.cn/gtizdqudsk.html

for x in a { print(x) }
来源：http://hz.andypj.xyz/gtoncnnpji.html

[T22] Swift：字典
来源：http://hz.hammf.cn/gtmsqzxbai.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj202588.top/gtphrrqwkz.html

[T23] Swift：函数
来源：http://hz.yangfankeji.com/gtbfxnsnyx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ehwqpu.com/gttbgkfqrn.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtdqcfgoqa.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yuxming.cn/gtauiibdiq.html

[T25] Swift：结构体
来源：http://hz.yuanzhike.top/gtiblyihff.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtybyzfcix.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gtkmwcufpf.html

class A: Base { override func f() {} }
来源：http://hz.nanxinkj.top/gtccsojxmt.html

[T27] Swift：错误处理
来源：http://hz.yj20258.top/gtgunaxbcc.html

do { try f() } catch { print(error) }
来源：http://hz.tian-w.cn/gtvdmyombh.html

[T28] Swift：枚举
来源：http://hz.xziqi.cn/gtmcollnfm.html

enum Color { case red, green }
来源：http://hz.yuxming.cn/gtzrwwrqfh.html

[T29] Swift：guard 提前返回
来源：http://hz.yuxming.cn/gtbtfydhor.html

guard let x = opt else { return }
来源：http://hz.tianlin.xyz/gtwjztgkwr.html

[T30] Swift：协议
来源：http://hz.sufxvd.cn/gtsjkboqvm.html

protocol Shape { func area() -> Double }
来源：http://hz.jlsjyb.cn/gtbisnpudv.html

[T31] Lua：Hello World
来源：http://hz.kuanghao11.cn/gtqpdmyeqq.html

print("Hello")
来源：http://hz.cheryme.top/gtmyenvtjo.html

[T32] Lua：局部变量
来源：http://hz.316326.xyz/gtrvfwnooo.html

local a = 1
来源：http://hz.hnqzz.top/gtvxgpfvod.html

[T33] Lua：表（数组）
来源：http://hz.sysykeji.top/gtoxkphmog.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.cheryme.top/gtlbeisekd.html

[T34] Lua：遍历表
来源：http://hz.shanyushiyangtech.top/gtathqbzzx.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtphpcdigb.html

[T35] Lua：字典表
来源：http://hz.zhixingplan.top/gtscdynzsw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yonumen.top/gtkggiwznm.html

[T36] Lua：函数
来源：http://hz.chenjidiqi.icu/gtilvbuqax.html

function add(a, b) return a + b end
来源：http://hz.aizwys.cn/gtuduwpcnt.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtnkvzwvnt.html

"a" .. "b"
来源：http://hz.ybcxt.top/gttnvrdpyt.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtmdoohkhs.html

if x > 0 then print("正") end
来源：http://hz.gogol.net.cn/gtjhhvqtlw.html

[T39] Lua：模式匹配
来源：http://hz.snrcjt.cn/gtvnqappno.html

string.find(s, "%d+")
来源：http://hz.chenjidiqi.icu/gtflgvfmbl.html

[T40] Lua：元表
来源：http://hz.chenlongwang.top/gttfksnlqh.html

setmetatable({}, { __index = base })
来源：http://hz.yj202588.top/gtzdmoljdj.html

[T41] Perl：Hello World
来源：http://hz.shzxlz.cn/gtazicnexw.html

print "Hello\n";
来源：http://hz.sysykeji.top/gtecylkssk.html

[T42] Perl：变量类型
来源：http://hz.tianlin.xyz/gtdkluafjg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.birdmap.top/gtgrwzlcxf.html

[T43] Perl：字符串插值
来源：http://hz.jqgufenzy.top/gtcyagwkyq.html

"值: $a"
来源：http://hz.chenjidiqi.icu/gtwfkuzfeu.html

[T44] Perl：条件
来源：http://hz.hfpthk.cn/gtjebsoiyw.html

if ($a > 0) { print "正"; }
来源：http://hz.ivvv.top/gtfjdqynha.html

[T45] Perl：数组遍历
来源：http://hz.jinyuanbaomall.cn/gtoyvkhflv.html

for my $x (@arr) { print $x; }
来源：http://hz.havefunace.top/gtfhjgmjox.html

[T46] Perl：哈希操作
来源：http://hz.yueranfly.top/gtptfyhdvm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.yangfankeji.com/gtvjtsqgjy.html

[T47] Perl：正则捕获
来源：http://hz.hongshengwenyu.top/gtighfakvf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.nwbrower.top/gtxvojywmr.html

[T48] Perl：正则替换
来源：http://hz.zhengqikj.top/gtwozupfek.html

$s =~ s/old/new/g;
来源：http://hz.sxryk.cn/gtnxbwzvjt.html

[T49] Perl：函数
来源：http://hz.svipenyu.cn/gthkioxaor.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.cucudq.cn/gtzncdvfsu.html

[T50] Perl：逐行读文件
来源：http://hz.tian-w.cn/gtitekmmgc.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangkeji.top/gtegqgailx.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.zdqjudy.top/gtorrncskv.html

[T51] Scala：Hello World
来源：http://hz.sufxvd.cn/gtgelurmuz.html

println("Hello")
来源：http://hz.yongpay.top/gttcxwpsoa.html

[T52] Scala：变量
来源：http://hz.chenlongwang.top/gtcuixfdkj.html

val a = 1;  var b = 2
来源：http://hz.aibaodan.cn/gtvczbbccy.html

[T53] Scala：字符串插值
来源：http://hz.chenjidiqi.icu/gtvwikngow.html

s"值: $b"
来源：http://hz.jinghuilouyu.cn/gtuwjzgizm.html

[T54] Scala：集合映射
来源：http://hz.cdnleiting.top/gthjusivct.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.chenzaomai.com/gtczrfmrwx.html

[T55] Scala：集合过滤
来源：http://hz.316326.xyz/gtibmegcvg.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.svipenyu.cn/gtkbcorkib.html

[T56] Scala：样例类
来源：http://hz.fzhhl.top/gtackzllcv.html

case class User(name: String, age: Int)
来源：http://hz.52xcode.cn/gtuphwjnrz.html

[T57] Scala：模式匹配
来源：http://hz.tian-w.cn/gtmyqimmmz.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.hongshengwenyu.top/gtzjvtpnsc.html

[T58] Scala：函数定义
来源：http://hz.zhixingplan.top/gtvrilhwbs.html


<!-- 参考信息 -->