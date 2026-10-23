代发 wailian999

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sljvllcp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pryrteiu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3pqtewxww.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3msgjbzzp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3jimnbcof.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3yhofxaym.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zqohyuok.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vyrujckc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ydzydbnd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ukbxmeuf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tndtzhze.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mzesfecq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3omfnvxaa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eprwslsk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qyslaans.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ycjbyury.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3rtyysmxg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3idhviegi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ozyusvnx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3wkuesjnf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3txttmydr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ikwbxrvi.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lcpabkms.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dttqmmhe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3txkjbynn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uenccror.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rkzlftxy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jyffgkyt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3nefdtitg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3vloigivg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xhtvilch.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lpxqrzmq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3buioidwu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ufqlzcqc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3eemqdwta.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfhjkt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sydwhvfy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gnpefbls.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3dqrlaqyk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3sexdstbz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3megpfdhz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ingiawpw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3lljmcojm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3kyjleqpk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ofqkslna.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gkzdaclm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ffbzhfyv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3arxjknsz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3nffqytar.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jubvcokk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtvosmhy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jjrxzeaa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3uhslwmsc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3olcqbeom.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pincsepf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gyclkafj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zktvoaiv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mefipkca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mceyrvlc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jbiporpi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3hhhhixkf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kwjvebze.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jqpoovoc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3phyqyneo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qzzcdgsr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugppsbhz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3oefffaji.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vxgikfio.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wenjzvvk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3amlbrepn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhnuxuli.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rqgbhonf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qinzhiql.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3irwzysxd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ugfabrcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amliazlt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3foumazrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkftbxyi.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hottohcs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wlpococd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezgciuct.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kmzszmwl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3eadecijm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xxkohbks.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3saimwiff.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vvoozbyf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ildnrjny.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fhlvlixp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3vwwwkmxj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ogxjqdeg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ohjzajuz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fhoyskbh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qzdsgdmc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvvjab.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wpqolaiy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3lvwkmfdh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwghqy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hfytmocq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlmket.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xybtvzdj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tinjmlyc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fasucwxr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hhgtaffq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3znmdlqjy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3evckmnvi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3tdfvelcr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3onmjnehg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jhlkidan.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3kgmaggyj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3skwrwiin.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3uuqmqyzk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3atyexabq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3udefqnst.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xnevjyzu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3czyvyakw.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3oecxxdkl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3yxtoofma.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uzwxbwmh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zsimsxvg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bnnqxifl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ijylotrr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3hxjlyzpf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bnnwwgdw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ihvaidif.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wdozhfyt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mmxgawbs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3gpoaqdfu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3oghpxahc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3nmkrvhjw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ebrzrugd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tcgbvkyu.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jznosusd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3qsmyeylb.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wmmqhqnq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqxahpcl.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3oymtcsxc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xuyvnhnk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lrarnppg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3lhgnldzc.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qtaaxcnp.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mvypvvwx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jfbnlifw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3bmoevsxr.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xfdhjkhy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vauifiqv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrhnrwd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3omkjqilj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3jzuleoix.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3groksnjh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3choisidk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3idclcxkj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3itjhlijc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3mhjcebpg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xmyujion.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3manwqzec.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3heipsolr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3nbytkhkh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfebmsmi.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3mnxcyztu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3vhoxakvk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3kbomlaxp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3vmycfnrz.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hqtzgfjl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3izywluwv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hulmylsy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hdsuujsu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3odorymgq.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3vmbpsupo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ktvherab.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uykdubew.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3woumaxhf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpakhwow.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gfrecghk.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mactrxnz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3jnebfqlt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mensasgs.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hdcbkvin.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wxxiakkh.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yikjoyhw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ciifofpz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qjzrlhxj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3yxqrnfqw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3erclmnqq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tcjpwxjq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gwccadvb.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mhijaowy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3qxcqwlka.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3cecluitj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ujixukhd.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3ehizdtqs.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wjszppvw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzkoytak.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rszbicfi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yjxsufmy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ufkdoojs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3uvasvzyh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjdjeude.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wcouolkk.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tehvwdlr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3aaxvxusn.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hrjfyoet.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3omdrmftb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3drdilaax.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pdurmpas.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ztddccov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oizhfqpj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3whridlxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkqaakji.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3htnxmtmz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qrgunrcs.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qrsxouow.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3vewdwjap.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3cxsrumrs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3cqxnxllh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3fgeaklmi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zdgkvfzy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3ypbswokg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3popjlwxz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3urbudenz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hufzhtrf.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3swanwmlg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkwizgb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3nwamwuxj.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gqgipgel.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3xzlyzcwm.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3lednankn.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tjqeniwl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zrhbqlos.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3uitusbqs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhycfqh.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rlrlsrva.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emwhcvpc.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3uouezrms.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3outaaheh.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3zqixqqro.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3uotntarw.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vtqejeec.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3lazusskj.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iicmqouu.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3azdrkdta.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wzhostep.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jiqheghs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3lpurqgkx.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3xooouvyk.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3jxmugmxu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3lelqjsui.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3jjeomnpm.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3avqooaix.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ynvqrbbg.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3mdilpodx.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3plqxqpam.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3glpohxra.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3newghake.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3wzqnnrsi.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3taofauqy.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jxczlbvl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3zcijfozc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3knmffajc.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3wqpgeatl.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rerjably.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3aqvettrq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3tdyxjapv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gcbswobd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3liizewmq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3srylxzhx.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3whgcmgnf.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3tlfopcso.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3qxyjqeei.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vklcuviz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xtnfclpd.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3paawhdyp.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3stbtjxfm.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zigpsdei.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3zvoyuwik.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3wuvqegel.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3gmmekrag.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3rjsoomwb.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zhakukcz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3kyxpogkr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3rlucsvhw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rzmxxjvq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3ikkcxxwp.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jnbazjro.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3neiwcjrj.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3obfmyyaz.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jmbdohfg.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3lyichhnm.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3fxuweald.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eppaozns.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3ytjpxhqj.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3omqunvgc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3cvqfcotw.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3qtrsaaxf.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3thvadtgq.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xidjnohu.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3nsxaiauv.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqwzfaqx.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxwwxila.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgfnji.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3onwgkmnw.html


<!-- 参考信息 -->