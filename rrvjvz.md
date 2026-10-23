代发 wailian999

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pqyfwhut.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lgjchzmi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3agfiwfox.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3rzmqyucl.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3afcqrdsp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nhmjnycg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gypglsuy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3wuljaqge.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3wvqpchbl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zwnusqrh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3aotfqbld.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3epcpffpg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tunsslyt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pimetnzh.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gxhwzgan.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3leksnrvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dblzmcha.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xvaubsyn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhopjbdb.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zklhsceu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yerbwthj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fwketzxu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3phlfunog.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3cvmpqpnd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ueoseese.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwglgopf.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wtdqviec.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dxkwfqwi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mkrobipp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3juylhwlx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3reqspblg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nibsuiju.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hyniyyhs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3msoigskt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ravalegd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lqaubffu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3txsfpgov.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cgiofzhe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pzcmmjtb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3gauydmva.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qxxrmbep.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dyhslayl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3emzvlkbr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ysxospxb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cwfotvwz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ysviisqn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pdhbxsby.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nrzvxmcw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qpriuqco.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfphfy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zffciifz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3eezhktte.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3obnvugtm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pqxgpwdk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wxyafmbn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iywmtepc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3pkrryycq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jxejpbfs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pauhdbrq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3etbskrmf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3wphjtrrq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mzsolvvk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mrrhrpwd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qhwwsisd.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ebmksrkc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3azfyusnx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vqxrcviw.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3irfjoino.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3nneajhpy.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3nmbifaop.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3paishsyc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3oxyrunwi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vrnuctft.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jzexacwb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wtfmfgtg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sgvhlipc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nyhdmgkh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xarroscq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3zeovqruy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qapqvobz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3byazwtva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hapaaade.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lybqhfel.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hnfhzxsu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3vnratggz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ogtdrexw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ogblipkw.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lunwabpk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ifwxaiku.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3okeyaiab.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qvvnxcgs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oychymxo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3verffvsn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mictbfza.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3jfilsdfq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mxlevsai.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3hvwmuthr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ympvzwjq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3fknrqktb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ogorqeqr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3roljecsf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ftkzukbp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3slteauqx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nwyvxihu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3pxfehuvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hxewvphn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nzddswwo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogruxeki.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dmgzklnp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fckywlob.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3feiaohdb.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vdevpega.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ayqriqxt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3mnmjikus.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ziaylrxt.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3maglafbm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lrddnwzv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gfifmqij.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3rhvuubqz.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3phdglydm.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3cxqihwsk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fytoorlk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3nbdkonoi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3jokyunyg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wdpzsnsh.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3suepnmgj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3owxzecra.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ijbaffwm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qvzkvxno.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fktajskr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lkvtdysz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rjflrhjl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3sobxdxgp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3owqtsyyw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3zsebiqav.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3xgucejud.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3abpwoxap.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3qvoteoca.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3unrsjkpy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3jjlwjbfd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3omaorigt.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tnrhsbdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3wmtsrqeo.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3utnnbdph.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3ylgmxnid.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3vrycgcrj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3wtaaexoe.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pkdhsahb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3irflsfmx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fylmyrlj.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pqnypzwz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jnsdtuhm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3wgtysqyg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3wlarhvbl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3totciepq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrulpppr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ssyezfnt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qdocyvfu.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ynbhrujv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xwgmhilx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ifitmjgy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3fkncwpas.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3fnurrcqp.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3rtmmqdmo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3xncxvqrt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cwyxhwrt.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3csdywkaq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3wnafpfer.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbitipyq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3vdbihkpb.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qvuermpu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3iwuehadb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3vwxfpgal.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3yhtbbeev.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3iyhmrjdp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3nmcbvnpx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pcstzqtr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ormabbad.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3uwvoojul.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozvsuwtu.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3ntcuujay.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3amusqlcl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jzmrrtus.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fhazoadu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vrtcqosn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3snxhurin.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xxjwkzac.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3nykgjgvr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3shoihwqv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jqbxmyhz.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3cbfnarlx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3mioicvnk.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxflxoco.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3fcvevupr.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cmvyytwx.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3eckiezxb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sjotcilj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3gtogvfvg.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3aayymdkt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ixeiiyjm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fvjnhmwf.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3ktgrjnue.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eoddqunp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3cympvicb.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3syxdpmvc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mthriduy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wrlpxmke.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qbzzyipu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3uuqlqeqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhlubfcv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3oyjlegjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdcpugsb.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3szoswgnr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hbtdooem.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3iftudouk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3dfqkorov.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nfgqimeu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fmrfgodh.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3zowdexwe.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qagswjvb.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3enpdngwq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bmeldrlv.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ncaxmpjw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3acspurra.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vubayfdq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3naokelgd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3gxavxvvm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3dernumkm.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3iistqyag.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3klnkedfn.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aquchvaq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3bhmvzkhz.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ybyzbnva.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3xjzdbfxe.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3tolylrne.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvltqpvv.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jkxjaqce.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghfcrgdn.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ruymgihb.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3quugdoxk.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3shngsiwc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3pxgjtnmg.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tjmowgwv.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjfwwso.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hyhoqyks.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3bihhmtge.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3phzxhttv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3sbabbzeo.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3gvxxufgc.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3evxrywzx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3fzdnufwg.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3pwkjviby.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ikgpbikc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqhszgzs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fduhhcfr.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3jdgipsny.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3lxyjaguy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kinjokxh.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3xdyawiwk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dwjsbqec.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3isdqymaq.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3rsmaaywj.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3menprtwm.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3qcwjiihn.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3kygpvsdn.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfcykrhh.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3rmufhgev.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3xlbschfr.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3auchrhnb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iqledkob.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3czivvpjp.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3mzztuavy.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ojsplfgm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3sbseshzj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdputh.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3jixlsveo.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tjsnzkla.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3xtrkcevg.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3hmmbxtat.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3homhbbcc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3krcyauni.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3nvmhpwzs.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qfdknwpj.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kezyvgve.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vfohmmpu.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3pjlsenez.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3aswwjsvw.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3mblbmrfu.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3kubuhvtu.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3amqmbpad.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3awlxwepv.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3iqjhbsps.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndqrqffg.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nhwmqpwu.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3meytnxvu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3yudhpdkt.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qhcgsgvn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3wjugaaww.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3mbmpqoty.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gggtmrvu.html


<!-- 参考信息 -->