代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3meajsyba.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3erkgzgey.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uyrsbtol.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gvasprhq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dflkimrj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3fxqslrin.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3glhlhkxu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvhhjdsc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ymzhmdiz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vvxyxbnv.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3vtxtbiqu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vcdjzuho.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3raxdozsz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vmigcncb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3icqjffgx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3jziqcfqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ilyipsme.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yhbjneqp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fqppqmym.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gcbhnujw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3owhddzup.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ksiyimxd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aeiyqvpl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3benkbelc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3paepcnxw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ychxeota.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3occfykwu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ofowpwug.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mitjzwcl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3apdoojdy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wiewsaqm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3qhtfzeqi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cznhztgu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3aczipqao.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3eryfgrxg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ofzvscsd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3mmgnaqme.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3smltzgnj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ytsebcow.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3xvbddgtv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xgdtfdxs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3krhzornf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3anrpddfm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3banwqnap.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uubapnlv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3trfyyupn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jshijnrw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3anxfzfpf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3nfsxocng.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ivpyhyvw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3soljszbr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gcdeglfu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3iaoqqgnq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3olwfcpyp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qooyihcy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3splgvbxu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3nnvgtixo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pfecuxrf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3auzdwlsc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3xrektmzj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pphvpnkf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3tsdjgxqw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3imgkqjck.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gafceeew.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wuckhcxx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3veuuaoeh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ajkzaqwl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ggozmehc.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qzqsehst.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ieeqtvew.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3zrjimokw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kilhwabp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rajupiru.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3jictdcob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tllyofcq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3fymwlkzc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gywchlrk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3aqifdduv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jwhuwrzo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3seelcelf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fplstiqe.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3lqhgwybh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3aksbdwqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grlenrgq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mahxlbgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhrndnlx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byxovldk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3byxtsbrx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqsvvoi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3olwcndez.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3msalilbm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jhwoqcmi.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3bbwqbfxx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ymbfhcac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3efpbbvwn.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzhptvwr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmiwcudc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sheqgwij.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tmzxbnmu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pwquwnnd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3swfustpe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yxotrxgb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3kswyhhaa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3twveesaa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rjwqqdoa.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3mhcbjebb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ijhkjjxj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3cuacuxkl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fbhpdjlh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3hfkrkdhy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3tgfaajmb.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vfzxnaqz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ropjflad.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iwjvtsts.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vmfwqhya.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uoeiqtgd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mdbovmvq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3njyxpjyl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gllypajv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3mliayjrq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3hdumykmz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hhtuqeqf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3uykrmpif.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ispaxkfx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yxfspxfy.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qtrvbebp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vvviapbv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pkqzfvoc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3aoyivayc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lrjagoqh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ytjgtdbt.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vsfewzwg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3bryjjwvq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uczfpdpv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3tzeerarm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hozbxvih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbfayax.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jesghove.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tidildgt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3huuhjycz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cyvnhxsa.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qtrhznzd.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ytgubtjp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tohqcdpe.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mxqonrda.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vxmcrjtc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cuhspdnv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3tfkjesxx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fhrwvcza.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3tgpwvkdd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3djubisus.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3szfezjvx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3csbckloc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cqejnlgf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3bwwfchjl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jtykrtjx.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3dykfucmz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3lufpqnak.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3kdjblyqx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lskgaqee.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3yfiawzbd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lbourbxl.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3cqqqdzfv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3afpnzomy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gsidfufp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ebdthclw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vyjzteds.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xfysvrbj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3vatirdsr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3eizunait.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3vlqnxirp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pneaixkd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3njkvtcjl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ufokmceq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3duslxmkt.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rgmktwrk.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3kvaniqxm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3awzmqmhg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qdqaekfl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyutoasc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wwhzuicp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3gttedgxs.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3suirfqxv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3dslatmjr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ruzfzxym.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhuowapg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yvvnggao.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tunxyivu.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tslggyap.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3cddtjjjc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ebgghlxy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qgqklhvb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ygeaftyz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kycarihs.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ditjqcvn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3euhgjvfx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgnneut.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3yioixwoa.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3smtlcrbh.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bvkzbjhw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3jwwqewjm.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qfpsjbcc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3pqrqizcz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3itxoldad.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3ikjlnien.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dhfqevpr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fqbypvyx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jouvxhko.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3ntnxunvf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3rbeffmth.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3hxpmvfkm.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bdwwlwqj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lbbgnphz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghazecof.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nbtfwiqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juempxlq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vhzzewjt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ruzsyxjb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nylntngf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3piubrscp.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3pxjiyzno.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3swsfcowi.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aaeiqjbp.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zksektph.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3pirxuwyv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3xiiaqcop.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3uldxztho.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lnihztpo.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3awezxjuf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3xgtgozwx.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3usrngksu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3ivthgoln.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mtrkqfen.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ibuolzir.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dvfcibkg.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bboinyfp.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hygcrjoa.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3lynzklip.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3eosrnaqx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3agqnfeeb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wtnxapta.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3avienjlk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnlfkmby.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3djfmpvpa.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3pvljmfsz.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3mohhkvac.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wtaqidda.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3jaxurtuh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3fwfrqkrv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tulvnwft.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3conswwaf.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lesfmgkq.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3nurrycyf.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3qwcnfqiz.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3tfdddrms.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pltlwcyv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3dmgtuheu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ckeakjjt.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ghplgezk.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3hpideljv.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cnthsgsk.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kjyiblpd.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3lfnhcork.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrjlfkk.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3qhlgkarb.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3yungnlxu.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qqnwcdoc.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3ddxwijqe.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3pjfpwlxj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3unahjrrn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lootohes.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3qgyzvlvu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gschrwpb.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3zzkjysgc.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3dueqzubi.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3hhpuuhlk.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hutvacub.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3awqddogt.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ahebcifu.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3mkertosy.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iawnivgr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3ocmertcd.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fmrrhvhn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3tgzaquhf.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3hgwvvxdp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3faearpjs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3njydrsho.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3iwrmouhq.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3otdupmpg.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ivvccvqi.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3sggyhdlm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3yjkutfob.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iqyqqfaf.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xebshcuz.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3fqioblpo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3courexhk.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lkfpnowp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3trmpmdbt.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vpoobmkq.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xtebkeqg.html


<!-- 参考信息 -->