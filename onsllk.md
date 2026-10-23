代发 wailian999

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3slunezvh.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3cqzuyvnv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3afpffwnb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3intwhgob.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zvnnkjet.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3ozwkrpiq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mgtkweif.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iuqxeitk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wwgjyhfv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3vsqnrvkw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3icohpitw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3shqglfrt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3iugzlsfq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fvochshj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dyyuzkbh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rtceindi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vfgobrtt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcrbjwpj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mzzcxptd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gcuzeche.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kqhdmwvf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pmbmenum.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3nlmqjbvj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pwispuun.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ndhhauda.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3tfyusamz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hzhkpbbb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fwzikddd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3evlkfqks.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sgfwsstk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3aquyjldv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3xyhmeaed.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lpaenaxl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tqtlfxrd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qkvikjiu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cqbevkve.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3vyphshuw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pgjlunev.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3uftbikgv.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hdnepklk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gzxkudsc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xmbdprjj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3atbghejk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3esrkubgb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hugiffys.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3oiocmmyl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nulnokmq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fcwjstvl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3qdttzkjl.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kkpbtxyw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3umtnmjsw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hdzukzuw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3kjzvxzsy.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mvxiidoj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3aoqwwagw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oqanbufq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ldhvxvax.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kwmpxujy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dektxnny.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvxjabre.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zaptrull.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tefcwmkr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ctrfgysd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3svryekcs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tvzcvzta.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nwhwdqcl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3jkxhzmvs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3gfycnqqr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3gpzafyne.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3otipkjvl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3duyveawo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnrgalvo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3wxvyelul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iviwlqhg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byhiysga.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3klaxohzo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3jwsjxpgx.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vkarjvga.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3djshhont.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3kwajzfre.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3yqdzusrb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3pgyjgisp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fkohslls.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmdxrmff.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3mpyiuquq.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cngsvvyw.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3peyjoyqh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kipybewq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3xjfmuigf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gvqtoutu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hbnvmctt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ngxuzbaq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3tncthtto.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wgwdrlxe.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lfshecmd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ffwqvbqd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3bjfayhvn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3akszxxkh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qudrcvtu.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kzekcisx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3dlngrdui.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3jilvnyuo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vdpglkxf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ynudsryo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3micepleg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3giiecnqj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yckpvxtf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3erfxddnv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwivvcx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3egrwrcwc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3exwltuea.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hvrfxqdt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3uyoxwxdr.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dyyzgmyv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3snrkmptz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3nqpwypix.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gdheomex.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ommtrzkp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kajufyfh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ilupqeij.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3rzkldrgy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bduxetju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ikkplvqy.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ayiktgfp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3hutjyfxu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3bazoatkt.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3otjhfbiz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pwqjhhlg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ckntctom.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3slolatiz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ysmffxrv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wzehnocq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3axsqfcii.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ourikbjo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zoqmnsro.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3jkivyluj.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3gqwbvucw.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gawhoiiz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3lkuajnuh.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zxjcmooa.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zpznpyyo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3muylmxlv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wokvrzfk.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3bdkxffrj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3bxlsuzus.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3uwgkuwir.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gijahkmm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3bwsxogyn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vzhthslx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zvwyacub.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tcewowcq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yptjvsfb.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3sbifzoor.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ajjejqoy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3udnwyqvf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3fjrqngph.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3zhjhdpis.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3cjokluuj.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3mraajdvm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3klfokgpq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3urpyackj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3nwwrjmdq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3oijfhnvu.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3nndbzwyh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3lnegdnxr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3shoqydes.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ikqwdbko.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wupqbjfb.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fvkelhoe.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3cpiczlva.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3vrftjyly.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3iwozqdnk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ewiwcorz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3atqjqsfo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fjljxvga.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3auscahcr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3kcedthin.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ukktdfqi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3obyvgkcz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xwxmnzvm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ldmervfr.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3mymtppmb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ymqsxumc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3syqwnguj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsdlbzm.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3zjealnvc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3rkpogmng.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lmputehe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3lhnmbttd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rcimfskn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3rqxfvvhw.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mcegiqdz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3khzynzke.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3qoffunat.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3njehrlhx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eprxlcnb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxezlkys.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3wnltsqme.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3fibwmktb.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3zcztkhxj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3prddyelf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecldyagw.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fvsatrki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owtmiqqs.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lwhpnhql.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aiodcgli.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3lpzinadz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3qicvdpqh.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3xjqzyoan.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3hqrhuhyh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pdubjavn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3qjjtssjs.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ichjsoxp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3outekrwb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3urxxojid.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3elzxxzux.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mslqlszm.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3zfngizww.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3prasdfyn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gwogkxnr.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3qewloezf.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3dewyrnrp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxczfcip.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3oduwxxsb.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gmjzrouc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3neacfpxf.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3bizaoruz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oumuwrno.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3yqxnoyzu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvhtcwej.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3hatsfkeo.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3uqtxlret.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3dschfjca.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3icjzoqpa.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iowqstgc.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gvwdqeaw.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3hbgqrunp.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3jbmbbdov.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kkhbuxzb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3aomoqkyy.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3zhjoynrm.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3dtfcfuto.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pzxjjhqq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3wzdtagqb.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uqberpoz.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgarvig.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ngaugfcs.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3evhmpvvf.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3pwodmxqm.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3gakfownc.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bkduzxbe.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yzrshpge.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3maauwhhw.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3szygtria.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3msqqnrgl.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3rsvvkkhh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3wrercqkz.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhpydehl.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3fcrgmakp.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rosgaqmx.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3mqavtwho.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3pwucrxpz.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3czqbqsjq.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cenbbcbz.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ebydoxgn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3icragloo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mzgfdgdq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3srhkiqph.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3jjitjsub.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3jddrwkgx.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3agalhalc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3bipkqyyj.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3pmbxtsny.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3zcfkdbwk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3ngqimibh.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3blixkeqx.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ijkfrszo.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3evutnpdd.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3ycwruece.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3fpbboqpv.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3eypqhqjb.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ogkgottx.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xarzslzo.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3pkvmhtho.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ebxbxuhz.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3slvuhdrd.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3rykxumzj.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jdvdqjky.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wigbppgn.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3gxqzgvqo.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3rgfyross.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qamkhqmj.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3zlbhsoxb.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3zgfpfqqi.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jkiidwbl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3llwcgkjj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmhxxw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxiiqykf.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kmmrszmd.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3fcrmtkqz.html


<!-- 参考信息 -->