代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3evlbomqp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jihtmirs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mntuxjzk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3mbtkuvvw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wciuwdtv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3wvxvpsdz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdtlujhe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3eauxmkdf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ebsdgrwi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mvvjwxhf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hbgrxhho.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uhpcpufe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qeololxb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bixwpzcf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jrirctsg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vvvkuvpm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iavcfgle.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jbefehrj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rcmikptw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3phjajhct.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sgxsedrt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxdkorbr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3irkpzkaz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qrlzsodb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3diktajez.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3wotkejks.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ucvxdalz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3erxhqwql.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3tnuepbep.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3eaoybmnq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qkdvaiwt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ebnmhtsp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bfiybfbs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3eifdyfbj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gqxipjsp.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3drmjnubw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vngjdrge.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3vegznriw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gngeavti.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nicwiquu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ssvjioym.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kumutequ.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3krnlldem.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ydozkska.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hcnkjmxu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gxgrthtv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ocqitytg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fiwgdgyo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sqsrwasx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgcqgewb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nlkjcpve.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3twtfgybh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qfxltcfx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hcufwgib.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vkcztwdv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ekpyyoft.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kuexhbqz.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3urvccrug.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qnjfozpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqrgzpmq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tfegbypq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjoojxfw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yctilzeo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3mcaxcuzz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ctrdsjro.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eawptpsb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ijcdcbpu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ddpgpnqf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pvgrddka.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3abrtwifc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3tmlvbzry.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvfgkpms.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ipzcpvtu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fiowhvgn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3qwsdksef.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ygkdkiss.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ngibwhzy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bjrjdnwp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nnnejwin.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tqacmcsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3lwaczrhy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3oefwfcjt.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkhovv.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bccakpji.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kxezjwnc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3cbdbzexj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ghmylmng.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3izhtvbro.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3esyjyigi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3funjbyyo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3enpokxdw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rxlvuryh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ryvvdumn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ymijrfzf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gjqngumo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wehzcdjk.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3axmnhams.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mzknrhuo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uvgucmqd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nibgarqs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ifbzmwyh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nijehasy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yqfhrzpu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3mptdsqgi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3stkvvnfz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3gtocatyh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kcecivsf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tjebhgid.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3beooworx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wbztrvxd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3mjjlushh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3cohupfsn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qswaeaua.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3zrwbxwkj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3raaulvuo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3dhgpfrko.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qirwuelj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3oidumdrl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3arhxybkt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vratruhz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ocqkcjlv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tpjwejdv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3vlgpdlwd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qzblpmnl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ovizlzvc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3wmkhfltd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3udmcppzo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tijrrdvn.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xgpsbgpr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3mbnpnqll.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vbinxzcb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3imnvxshj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3xmttjkgp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3utwmtoic.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nucrkyhf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycipjeiz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bqqdumer.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dvdziozf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3xnbjmpzf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3orsiwyeh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mbwabxin.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tkjkmzer.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mdelaxvd.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3khvgisjd.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3tnjkhehg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3daptgrsb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fowemhlg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wumecpns.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3qgpaqnlj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3pqrovkwi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3ysuqkzmq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rnmymsmt.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3jazmchcn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lxzlmmgp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3yuohksxm.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhetrku.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3srxseonn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ttdmcvzg.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ecpdilde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3crkyzizk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kmigxymq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3pucztnkc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xocpokrx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3bmuonsse.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hkwiefwe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ramkmhfy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ehkrendb.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3lifesaas.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qzvcaytc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ehuuyigi.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3nfnirvql.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vrotvlia.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzfgizix.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gsvtvdva.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3atyxckus.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3kgvrumel.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3inhjiqka.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3cguxsyud.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3wtyaldmr.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mrctpzsc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpkjcqvq.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ceqlyxwe.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3bsmtscmt.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3zzdrwpbh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkkqunu.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uyvkywgf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fpjlminj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rlontfuu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dptnueds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qytlcxpq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ixwvycui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jctspsic.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ntdepmzs.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rrmumoxh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3rfkhhhqr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3idpfxnyd.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3zgqeffae.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ulaxxtnk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3letxpkrl.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3dzdqbmfl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3hzcfueas.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3fkzjjdym.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ndkssflp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3usbvxjav.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3iwvkjqun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3lyujxwbb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3vqolvrto.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3yifhdoxl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3okkqxlnf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3rfuhcepv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tiokdnct.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3ngjniwyf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3abwjrjkr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzhmrae.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3jkxoaqha.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ubxnzpke.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ypottvdj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3ohtxyeek.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3beeyekcg.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qrgnlrue.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3rigfhpwj.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pjsgfbpj.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvfsxs.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3oxhlffpd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3htuqilqy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccnzvzgr.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3iaeresxm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3oewozyqx.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3hfbmgaia.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3npifrrbh.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ijmbieau.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3bqcttlix.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3blbpwdtp.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3wytxpbez.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3zxpcjqez.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qnbktzml.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qurnwtre.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zgnultfc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3eejejahz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ltjrazpr.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3tzjvjvzg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3cxmlqnbl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3eqgiutha.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3fdxbyirc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3rvsrwfnn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmndtcd.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vrctcohr.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3unycojpj.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3iauuvwva.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3oolgwqed.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3bmnrdbaw.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3qtghdebd.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dccypzyh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3pvqpiubh.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3smhgosiu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3qkghrjwi.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3lccfvpeb.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3usvepvfz.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3whkwbose.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3dzljcbhe.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zfivxwnl.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvuenopl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3efwhlxvm.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3znwuakzj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3bidrycec.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qjvzifhp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3vsbwbpho.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3oysqigwj.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3fcbwgulf.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3qprwxveh.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mdnkhuln.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ssaruhtt.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uhwxazua.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ywdmbkbv.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3kiwpqqar.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qccpcclu.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ytqokzxb.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3twgnaolw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3evdvwgva.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3dwwdlpkf.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wzgmvwzp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlcnowyb.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ybgksokg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3ncmjdusq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3avkzhbik.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuaujgto.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3lrmrvhhb.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3lfcuvbhy.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3yzzjndgd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edbsfzpz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lnrcukom.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3wzlqujtz.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbuuqmqx.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dsijxoyy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nqehuspo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pajocmtl.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3qwvupfqc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xwpsvbad.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3heqmtvpe.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3bdezmvda.html


<!-- 参考信息 -->