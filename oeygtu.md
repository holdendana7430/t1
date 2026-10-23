代发 wailian999

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uezjdlkb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3dziatjee.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fwywshzq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zlgpsekr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3riqvfzrl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3khcjbqoh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eoawqyrs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmhisgnj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dgwvatit.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vwqpnicp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hhrcddlf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3abkkight.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rnokbjru.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rrjlttlw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hfopxvhp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kdkjmsit.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ugnoqyde.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3xyppwanz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3sruxipbl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mxviclea.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3oqeuexzu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3sjhzdfbz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwrolszz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fxrdbigc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3clrdiwvd.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3niugzdga.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zlwophmc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3oazqqvdo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dpkqepsa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3idhgizlb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nakvtcfp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lsijlwaf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ijzdswga.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3scmeehjl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qjykzztf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xgvtpvqm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ziiszyen.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkhcvsxo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3pfyoxydz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hgtdhhsv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ojaifnta.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ihbejayk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3namwuwpi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nqizbdfx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vikovefs.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3cdmgzhyd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zojlctin.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3dwamzeyk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yvutfwcj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hvfnkyvj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3atiggkle.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3nhndfkfg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bbykxzqx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3hpkplerv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ocxktoqk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dxvrrccn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jqigtsib.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fakysfcl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ncnobaty.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3lobejuve.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3taefkswi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3mvyzvusz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3drprcixv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jpdfeaio.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3debrcduh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3btskryjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mkbxussk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qsaatfxo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ubnfvhej.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3hemgyekd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aveoerpc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xaoprjor.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dveywise.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3dtbdmcls.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3chiklgmv.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vqklqpqo.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3haryxnvu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3eiieeguz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3okibtxwr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtxisf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3lspjnnwp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3snpnrbqz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xneaktvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckihkdoh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3dwnwnrxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukkhouej.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cotfzsyp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3easpmswu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3flgarjss.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pflakptz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3bobalpsx.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kefsmtor.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hrqydfzd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nztwcifq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bwoncbor.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gfgfsoyo.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehsntsil.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rqtyqviv.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uomybsbl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gtvmxdcd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3laetxgjx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qphgogng.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3iohpzjtf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3oqyxwsiv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3daerokza.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nzjqcoqk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3revazhhy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqkbmndw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rylbexjn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3fqwuzbtz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lshzviyj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lgogxdpg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ewqmznyh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3thuygpar.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hcsgwmwu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rqvjuzgf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3fbxflpnd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3nrhewyjx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uwxvksph.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fesavqoa.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmfcpkk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cusjkfam.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3wmufktgo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3doezquvs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3kfhvyrhh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ebszuwua.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3iktvkorn.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3zxpywjlw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ypfmuisg.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ooacrosz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3btwtfxuv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vonfjwrq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3hawaevcj.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3fjhonifq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pbdrjkeo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3burtchkt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tmqvmlel.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rzzxuucn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3muxbitol.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vamznoyr.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3avfnshmm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wxrrlnqp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3seoejpth.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3exkopgbg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dlmucbwn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3oxuexjrm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3axuenxhn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hoetltjh.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3whwinsfa.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3kttzmvbd.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dqhvwiyv.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3haeiljgs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3roeivcko.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3qbfsnkea.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rahyscun.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hvtanatg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jjtbnemq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qpudjqle.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3tneejhjf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3leggtphi.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kczxinpu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rkfsluwb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3wxquensc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lwnpoqwz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3edfudfga.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bnjsxotf.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qyjiermk.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lmhsbjjb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3wchcwuxr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3hbousorq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yqjvolej.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pztdfhnd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvsycjeo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3cxawxrzc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nmyttkmc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3oybzloof.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ufacawlw.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3iavxfvim.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3polknljb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3xfqcsvrj.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zmomqbtv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3ezkunqph.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ykchhmeq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3glrqqzsm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3osfygdvl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qmvahvhr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3enzlkyqf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3flpbnpxb.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3ryxfvghs.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eiqinnga.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3nfmxukaq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3wtithhpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3khrqkijb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3uqayinwd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3soiosoxk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ylwmgdrr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3imbejbrc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3erodgffq.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fdmwnbrs.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3qtialmvb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3juvmmzvp.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3vfvhpruf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3tepwgywd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3eihiegja.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvivfmri.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rdpcqhpw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3trmiqlxn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3sljudnxe.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3drykheaw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3mmlsvbir.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3asflnbwp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3coomuwpb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3jtgxvshp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wesbrxuo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rigqbriq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzepevep.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3sjhaaime.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3darayvzv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cnxmmydw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3wkmxmkdg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ohtlgxsz.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3gbrpojwt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eomfrpbu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3iyedtotm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xhkoybop.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3tmffzjlg.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nqqhkvdw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zjkvhbgy.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3adkupicv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ayvnownh.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfazoo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3igsqmcbu.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3vhscnwee.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3pqanrqir.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3onbckvtr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3srubwdqi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lnauajze.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3runnmhce.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3ysoyweoe.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mqpscsyn.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3jkphkxic.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3exildtwu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3fhqraffa.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3slqodwbz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3ifvmygij.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3eubqlyud.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3svauoyhn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hotcehly.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3byxaegno.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3tbcqwtse.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3izvqnlbt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3thwhakhh.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3osshbyxw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lttplnwv.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3igbhnvzq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hknewbbp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aouzvhww.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jdircldm.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3spbqxkby.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3vffttaqv.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfdqzmqz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wciwklll.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uxfbjzjg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vwpgfdji.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3dplpytbw.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3vzcuqjlm.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3arwqjfis.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3vqsyqveb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tzmpcbsj.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3jzbxatlj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ibdilnaf.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3vxlppmkp.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kxwbfihw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3naxgyhhk.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3soppwnff.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3lahkgzbo.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3luwtmnvt.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3bhjjaxmi.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxvuckcn.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt3eatkxjxl.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3horwkxen.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3krwwzwwj.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hydgieji.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3rwmtwsgn.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3tbkmacdq.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qjktbucw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3npkjjqgt.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3mosueowl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xmikwzru.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3sxxdeybz.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3frhroqnm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3zgscbqll.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3jbhilmjt.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3vciadvre.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jyqvrsox.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3eyuifyvu.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3msqywyop.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zeeatpgr.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3qdcgjten.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3sfbrfzcd.html


<!-- 参考信息 -->